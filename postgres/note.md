## Install PostgreSQL
To install PostgreSQL, run the following command in the command prompt:

```sh
sudo apt install postgresql
```

## Configure PostgreSQL
The database service is automatically configured with viable defaults, but can be customised based on your specific needs.

By default, only connections from the local system are allowed. To enable all other computers to connect to your PostgreSQL server, edit the file /etc/postgresql/*/main/postgresql.conf. Locate the line: #listen_addresses = ‘localhost’ and change it to *:

```txt
listen_addresses = '*'
```

> Note: ‘*’ will allow all available IP interfaces (IPv4 and IPv6), to only listen for IPv4 set 0.0.0.0 while ‘::’ allows listening for all IPv6 addresses.
