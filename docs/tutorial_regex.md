# Regular expressions: Just the basics
## What are they?
Regular expressions are a fancy way of matching patterns in text. This gives you a more powerful tool to do search and replace, which can be especially handy for cleaning data.

![XKCD comic on regex](https://imgs.xkcd.com/comics/regular_expressions.png)  
[XKCD comic on regex](https://xkcd.com/208/)
## Where can I use regex?
- Open Refine
- LibreOffice Calc (which is why I often prefer it over Excel)
- Command line with grep
- And more!
## How do I use them?
Like your normal search in MS Word or "find in page" in a browser, you type the string you are looking for. But instead of just the letters, numbers, punctuation, and symbols on your keyboard, you have other "symbols" you can type too in order to specify what you're looking for. (Skip down to [Examples](#Examples) to see some)
## Boundaries
- `^` start of a string
- `$`end of a string
- `\b` word boundary

## Basic content characters
- `.` any character
- `[]` creates character class
	- In other words, look for any of the things in here. Can list all the things or create a range using a hyphen
	- `[abc]` a single character of a, b, or c (change to make any characters you want)
	- `[a-z]` a character between a and z (inclusive)
	- `[a-zA-Z]` a character between a to z and A to Z (inclusive)
	- `[0-9]` numbers between 0 and 9 (inclusive)
	- `[^abc]` a character that is not a, b, or c
	- `[^a-z]` a character not in the range a to z (inclusive)
- `()` creates pattern to match
	- (abc) matches 'abc' but not 'cba'
- a|b match a or b
- `\s` any whitespace character
	- If you know there are only "normal" spaces, you can just type a space
- \\S any non-white space character
- `\d` any digit
- `\D` any non-digit
- `\w` any word character
- `\W `any non-word character
## Escaping characters
Escaping: when you need to type a character that the computer thinks is part of the programming language (e.g. `\` in this case) and make the computer understand that it is content (a literal). Put a `\` in front of a character you need to escape
Use `\\` to escape `\`. 
Use `\/` to escape `/`
Use `\.` to escape `.`
## Modifiers
"a" here is meant to be any character
- `a? `0 or 1 of a
- `a*` 0 or more of a
	- This means that `.*` means "Match any character"
- `a+` 1 or more of a
- `a{3} `exactly 3 of a in a row
- `a{3,}` 3 or more of a in a row
- `a{3,6}` between exactly 3 and 6 of a in a row
## Testing tools
[Regex101](https://regex101.com/) (Alex's preference)  
[Regexr](https://regexr.com/)
## Examples
- Match single white space from the end of a string: 
	- `\s$`
	- `\s{1}$`
- Match all whitespace at the end of a string:
	- `\s+$` (1 or more whitespaces before end of line)
	- `\s*$` (0 or more whitespaces before end of line)
- Match all whitespace at beginning of a string:
	- `^\s+`
- Match `/ ` at end of a line
	- `\/ $`
	- `\/\s$`
- Match all the days of the week beginning beginning with T
	- `^T.*day$` (assuming list of days on separate lines)
	- `T[a-z]*day\b` (assuming are not on separate lines)
- Match the letters a, b, and c wherever they occur
	- `[abc]`
		- Try with: "January February March April May June July August September October November December"
- Match the pattern 'abc' in lowercase
	- `(abc)`
		- Try with: "January February March April May June July August September October November December abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWYZ"
- Match the pattern 'abc' regardless of case
	- `(abc|ABC)`
- Text patterns
	- `[ab]{2}` will match aa, bb, ab, ba and not ac, cc, bc
	- `abc{1,3}` will match abc abcc abccc
		- In the string "abc abcc abccc abcccc", `abc[1,3]` will match the bolded text here "**abc abcc abccc abccc**c"
		- In the string "abc abcc abccc abcccc", `abc[1,3]\b` (have added word boundary) will match the bolded text here "**abc abcc abccc** abcccc"
	- `a(bc){1,2}` will match abc or abcbc
	- `a(bc|cb)` will match abc or acb

## Further reading
[Wikipedia: Regular Expressions](https://en.wikipedia.org/wiki/Regular_expression)  
[Regular Expressions Quick Start](https://www.regular-expressions.info/quickstart.html)  
[Jonny Fox, Regex tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)  
[Loyola Marymount Explanation of Regexes](https://cs.lmu.edu/~ray/notes/regex/)  
