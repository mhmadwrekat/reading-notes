# Automation

**Regular Expressions in Python**

In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:

    import re


The re library in Python provides several functions that make it a skill worth mastering. You will see some of them closely in this tutorial.

**Wild Card Characters : Special Characters**

Special characters are characters that do not 
match themselves as seen but have a special 
meaning when used in a regular expression. 

For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.

make use of two functions namely : ***search()*** and 
***group()*** .

With the search function, you scan through the 
given string/sequence, looking for the first 
location where the regular expression produces a 
match.

The group function returns the string matched by . 

---

**.** -> A period. Matches any single character except the newline character.

        ```
        re.search(r'Co.k.e', 'Cookie').group()
        ```
        `'Cookie'`

**^** -> A caret. Matches the start of the string.

        `re.search(r'^Eat', "Eat cake!").group()`
        `'Eat'`

**$** -> Matches the end of string.

        ```
        re.search(r'cake$', "Cake! Let's eat cake").group()
        ```
        `'cake'`

**\[abc\]** ->  Matches a or b or c.
**\[a-zA-Z0-9\]** ->  Matches any letter from (a to z) or (A to Z) or (0 to 9).

        ```
        re.search(r'[0-6]', 'Number: 5').group()
        ```
        `'5'`

**\\** ->  Backslash .

---
- If the character following the backslash is a recognized escape character, then the special meaning of the term is taken (Scenario 1)
- Else if the character following the \ is not a recognized escape character, then the \ is treated like any other character and passed through (Scenario 2).
- \ can be used in front of all the metacharacters to remove their special meaning (Scenario 3).

        ```
        re.search(r'Just a \regular character', 'Just a \regular character').group()
        ```
        `'Just a \regular character'`

**\w** ->  Lowercase 'w'. Matches any single letter, digit, or underscore.

**\W** -> Uppercase 'W'. Matches any character not part of \w (lowercase w).

        ```
        print("Lowercase w:", re.search(r'Co\wk\we', 'Cookie').group())
        ```
    `Lowercase w: Cookie`

**\s** -> Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return.

**\S** -> Uppercase 'S'. Matches any character not part of \s (lowercase s).

        ```
        print("Lowercase s:", re.search(r'Eat\scake', 'Eat cake').group())
        ```
        `Lowercase s: Eat cake`

**\t** Lowercase t. Matches tab.

**\n** Lowercase n. Matches newline.

**\r** Lowercase r. Matches return.

**\A** Uppercase a. Matches only at the start of the string. Works across multiple lines as well.

**\Z** Uppercase z. Matches only at the end of the string.

TIP: ^ and \A are effectively the same, and so are $ and \Z. Except when dealing with MULTILINE mode. Learn more about it in the flags section.

**\b** Lowercase b. Matches only the beginning or end of the word.

        ```
        print("\\t (TAB) example: ", re.search(r'Eat\tcake', 'Eat    cake').group())
        ```
        `\t (TAB) example:  Eat    cake`

---
## Repetitions

**\+** Checks if the preceding character appears one or more times starting from that position.

        ```
        re.search(r'Co+kie', 'Cooookie').group()
        ```
        `'Cooookie'`

**\*** Checks if the preceding character appears zero or more times starting from that position.

        ```
        re.search(r'Ca*o*kie', 'Cookie').group()
        ```
        `'Cookie'`

**?** Checks if the preceding character appears exactly zero or one time starting from that position.

        ```
        re.search(r'Colou?r', 'Color').group()
        ```
        `'Color'`

`{x}` Repeat exactly x number of times.

`{x,}` Repeat at least x times or more.

`{x, y}` Repeat at least x times but no more than y times.


## Basic Patterns: Ordinary Characters

You can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions.

Ordinary characters can be used to perform simple exact matches:

        ```
        pattern = r"Cookie"
        sequence = "Cookie"
        if re.match(pattern, sequence):
            print("Match!")
        else: print("Not a match!")
        ```

        `Match!`

- Most alphabets and characters will match themselves, as you saw in the example.

- The match() function returns a match object if the text matches the pattern. Otherwise, it returns None. The re module also contains several other functions, and you will learn some of them later on in the tutorial.

---
## Copying Files
**copyfile()** copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file .

    #shutil_copyfile.py
    import glob
    import shutil

    print('BEFORE:', glob.glob('shutil_copyfile.*'))

    shutil.copyfile('shutil_copyfile.py', 'shutil_copyfile.py.copy')

    print('AFTER:', glob.glob('shutil_copyfile.*'))

Because the function opens the input file for reading, regardless of its type, special files (such as Unix device nodes) cannot be copied as new special files with **copyfile()**.

    $ python3 shutil_copyfile.py

    BEFORE: ['shutil_copyfile.py']
    AFTER: ['shutil_copyfile.py', 'shutil_copyfile.py.copy']

![Automation](https://jit.at/wp-content/uploads/2020/05/3.jpg)


---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>