- . - Any one character
- .* - Match any number of previous (including 0)
- \ - Escape something
- \+ - Match any number of previous
- $ - End of the line
- ^ - Beginning of the line
- \S - Any non-whitespace character
- \s - Any whitespace character
- [a-z] - Any lowercase letter
- [A-Z] - Any uppercase letter
- [0-9] - Any digit
- [A-Za-z] - Any letter
- ? - optional

Example to match any email address - "\S\+@\S\+\.[A-Za-z]\+"

Example to match a line that start with capital letter and end with capital letter - "^[A-Z]*$"
