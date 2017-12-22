## RegEx cheatsheet

Meta characters:     `. ^ $ * ? { [ \ | ( )
`

Class :`[abc], [a-z], [^a-z]`

`[akm$]`= matches for 'a', 'k', 'm', '$' and their
complementing also possible
 
`\` : backslash very imp; used to escape the meta characters like if '[' needed to be escaped, `\[`

### Some special predefined sequences

`\d` = any decimal digit; [0-9]

`\D` = non digit [^0-9]

`\s` = any whitespace characters[  \t\n\r\f\v]

`\S` = non whitespace characters[^ \t\n\r\f\v]

`\w` = matches any alphanumeric chracters[a-zA-Z0-9]

`\W`= non-alphanumeric[^a-zA-Z0-9]

These sequences can be included inside a character class like: [\s,.]
`'.'` :  it matches anything except newline characters

### repeating:

`*` = either zero or more times

`+` = either one or more times

`?` = either one or zero times: `home-?brew` matches 'homebrew' and 'home-brew'

`{m, n}` = at least 'm' repetitions, at most 'n' repetitions

example: `a/{1,3}b` will match 'a/b', 'a//b', 'a///b', it wont match 'ab' or 'a////b'

### {m,n} other types:
 
`{0, }` = its like '*'

{`0,1}` = like '?'


