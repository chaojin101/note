| Pattern | Meaning                                        | Example          | Matches                                      |       |                |
| ------- | ---------------------------------------------- | ---------------- | -------------------------------------------- | ----- | -------------- |
| `abc`   | Exact string "abc"                             | `abc`            | "abc" in "abcde", but not in "ab"            |       |                |
| `.`     | Any single character                           | `a.c`            | "abc", "a7c", "a-c"                          |       |                |
| `\d`    | Any digit (0-9)                                | `\d\d`           | "12", "34", "00"                             |       |                |
| `\w`    | Any word character (letter, digit, underscore) | `\w+`            | "hello", "var1", "abc\_def"                  |       |                |
| `\s`    | Any whitespace (space, tab, newline)           | `a\s+b`          | "a b", "a    b", "a\tb"                      |       |                |
| `^`     | Start of string                                | `^hello`         | Matches "hello world" but not "say hello"    |       |                |
| `$`     | End of string                                  | `world$`         | Matches "hello world" but not "worldwide"    |       |                |
| `*`     | 0 or more repetitions                          | `a*b`            | "b", "ab", "aaab"                            |       |                |
| `+`     | 1 or more repetitions                          | `a+b`            | "ab", "aaab" but not "b"                     |       |                |
| `?`     | 0 or 1 repetition (optional)                   | `colou?r`        | "color", "colour"                            |       |                |
| `[]`    | Any one character inside brackets              | `[abc]`          | "a", "b", or "c" but not "d"                 |       |                |
| `()`    | Grouping                                       | `(ab)+`          | "ab", "abab", "ababab"                       |       |                |
| `\b`    | Word boundary (start or end of word)           | `\bword\b`       | Matches "word" in "a word here", not "sword" |       |                |
