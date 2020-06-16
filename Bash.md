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
# Reserved Keywords
- `$1` - `$9` : represent 1 to 9 argument.
- `$0` : represent name of the script
- `$?` : represent error code of the last command.
- `$_` or `!!` : represent previous last command.
-
