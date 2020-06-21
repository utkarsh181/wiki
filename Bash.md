# Intro To Bash Scripting

# Assignment
```
foo=bar # Look for there should be no spaces between foo and bar.
```
If we put write foo = bar it will act as if we are passing '=' and 'bar' as argument to foo command.

# Output
Bash provide mainly two function to  to output .
```
echo $foo # echo is kind of limited because of escape sequence and platform dependent.

printf $foo # printf works liks C version of printf and a much mature and platform independent.
```

# Difference between ' and "
There are two ways of defining strings in bash.
```
printf "This will expand $foo"

printf 'This will expand $foo'
```
# Logical Operators
These operators can we used in if...else and switch-case statement but they can be used to chain command also which make them unique and worth taking notes.

- ; : used to chain command together
	```
	ls ; printf "Listing out directory";
	```
For the next set of operators keep short circuiting of operators in mind.

- && : used to chain command which will run if first command is true and doesn't run if first command fails.
	```
	cd Documents && printf "We are in Document Directory"

	cd notExist && printf "We are in notExist Directory"
	```
- || : used to chain command which will run if first command is false and doesn't run if first command true.
	```
	cd Documents || printf "We are in Document Directory"

	cd notExist || printf "We are in notExist Directory"
	```
- & : this can be used to perform something called parallel processing or run multiple command in parallel.
	```
	sleep 5 & printf "All done"

	```
- man test : gives brief overview of values that you can use to compare value.

# Reserved Keywords
- `$1` - `$9` : represent 1 to 9 argument.
- `$0` : represent name of the script
- `$?` : represent error code of the last command.
	Error code 0(ie think in terms of binary representation on 0 , all bits are down) represent everything worked well and anything other than zero means there is some error with the program.
- `$_` or `!!` : represent previous last command.
- `$$` : represent pid.

# Using Output
To use output of a command .
```
printf "We are in $(pwd)"
```
# Redirection
[Bash Redirection Explained](https://catonmat.net/bash-one-liners-explained-part-three)
- 0 - Points to stdout
- 1 - Points to stdin
- 2 - Points to stderr

The special file /dev/null discards all data written to it.

```
# Both of these are same.
libreoffice &>/dev/null
libreoffice 1>/dev/null 2>&1
```
Use of stdin -

```
cat <(ls) <(ls..)
```

# Unknow Interpreter

If location of interpretor in unknown then we can use env command :
```
#!/usr/bin/env python OR #!/usr/bin/env bash
```
# Easy form of man

'tldr' are easy form of man pages which are intuitive and easy to use.

# Globbing
