# Strings
Strings are values made up of text and can contain letters, numbers, symbols, punctuation, and even emoji.

Strings are contained within a pair of either single quotation marks '' or double quotation marks "".

EXAMPLE
```
'This is a string. 👏';
"This is the 2nd string. 💁";
```

## Enclosing quotation marks
Let’s say you’re trying to use quotation marks inside a string. You’ll need to use opposite quotation marks inside and outside. That means strings containing single quotes need to use double quotes and strings containing double quotes need to use single quotes.

```
"It's six o'clock.";
'Remember to say "please" and "thank you."';
```
Alternatively, you can use a backslash \ to escape the quotation marks. This lets JavaScript know in advance that you want to use a special character.
Here’s what that looks like reusing the examples above:

```
'It\'s six o\'clock.';
"Remember to say \"please\" and \"thank you.\"";
```

Properties and methods
Strings have their own built-in variables and functions, also known as properties and methods. Here are some of the most common ones.

length
A string’s length property keeps track of how many characters it has.

```
"caterpillar".length;
OUTPUT
11
```

toLowerCase
A string’s toLowerCase method returns a copy of the string with its letters converted to lowercase. Numbers, symbols, and other characters are not affected.

```
"THE KIDS".toLowerCase();
OUTPUT
"the kids"
```

toUpperCase
A string’s toUpperCase method returns a copy of the string with its letters converted to capitals. Numbers, symbols, and other characters are not affected.

```
"I wish I were big.".toUpperCase();
OUTPUT
"I WISH I WERE BIG."
```

trim
A string’s trim method returns a copy of the string with beginning and ending whitespace characters removed.

```
"   but keep the middle spaces   ".trim();
OUTPUT
"but keep the middle spaces"
```
