---
aliases:
  - regex
---

#prog 

Regular expressions, also known as regex, are powerful tools for pattern matching and searching in strings. They provide a concise and flexible way to specify patterns of text that you want to match. In [[Python]], regular expressions are available through the `re` module.

## Intro Comp Definition:

- the string $\emptyset$ is a regular expression denoting the empty language $\emptyset$
- For any letter a in E, "a" is a regular expression, denoting the language {a}. Note that this language contains exactly one word and that this word contains exactly one letter.
- If "$S$" and "$T$ " are regular expressions denoting languages $L (S )$ and $L (T )$ respectively, then "$S + T$" is a regular expression denoting the language $L (S) \cup L (T )$.
- If "$S$" and "$T$" are regular expressions denoting $L(S)$ and $L(T)$ as above, then "$ST$" is a regular expression denoting the concatenation product of $L(S)$ and $L(T)$. This product is the language of all strings that can be written as $uv$, where $u$ is a string in $L(S)$ and $v$ is a string in $L(T)$.
- If "$S$" is a regular expression denoting the language $L(S)$, "$S*$" is a regular expression denoting the [[Kleene star]] of $L(S)$. The [[Kleene star]] of $L(S)$ is the language of all strings that can be made by concatenating together 0 or more strings each of which is in $L(S)$ 

## Key Concepts and Keywords

- Pattern: A regular expression pattern is a sequence of characters that defines the search pattern.
- Match: A match is the result of applying a regular expression pattern to a string. It represents the occurrence of the pattern within the string.
- Metacharacters: Metacharacters are special characters that have a specific meaning in regular expressions. Examples include `.` (dot) which matches any character except a newline, `*` which matches zero or more occurrences of the preceding character or group, and `+` which matches one or more occurrences.
- Character classes: Character classes allow you to specify sets or ranges of characters to match. For example, `[abc]` matches either 'a', 'b', or 'c'.
- Anchors: Anchors are used to match positions rather than actual characters. The `^` anchor matches the start of a string, while the `$` anchor matches the end of a string.
- Groups and capturing: Groups allow you to group multiple characters together and apply operations on them as a whole. Capturing groups also capture the matched substring for later use.
Certainly! Here's a concise atomic note on regular expressions in [[Python]]:

---
![[Pasted image 20240425185227.png]]
# In [[python]]

1. **Module:** [[Python]]'s `re` module provides support for regular expressions.

2. **Basic Functions:**
    - `re.search(pattern, string)`: Searches for the first occurrence of a pattern in a string.
    - `re.match(pattern, string)`: Checks if the pattern occurs at the beginning of the string.
    - `re.findall(pattern, string)`: Returns a list of all occurrences of the pattern in the string.

3. **Patterns:**
    - **Literal Characters:** Match characters exactly (e.g., `r"abc"` matches "abc").
    - **Metacharacters:**
        - `.`: Matches any character except a newline.
        - `^`: Anchors the regex at the start of the string.
        - `$`: Anchors the regex at the end of the string.
        - `*`, `+`, `?`: Match 0 or more, 1 or more, or 0 or 1 occurrences of the preceding element, respectively.
        - `[]`: Specifies a character [[Class]] (e.g., `[a-z]` matches any lowercase letter).
        - `|`: Acts like an OR operator (e.g., `A|B` matches either "A" or "B").

4. **Quantifiers:**
    - `{n}`: Matches exactly n occurrences.
    - `{n,}`: Matches n or more occurrences.
    - `{n,m}`: Matches between n and m occurrences.

5. **Modifiers:**
    - `re.IGNORECASE` or `re.I`: Performs case-insensitive matching.
    - `re.MULTILINE` or `re.M`: Anchors (`^` and `$`) match the start/end of each line.

6. **Groups:**
    - `( )`: Groups regular expressions.
    - `\number`: Backreference to a group (e.g., `\1` references the first group).

7. **Escape Characters:**
    - `\`: Escapes a metacharacter (e.g., `\.`, `\\`).

8. **Lookahead and Lookbehind:**
    - `(?=pattern)`: Positive lookahead, matches if the pattern is followed by the current position.
    - `(?!pattern)`: Negative lookahead, matches if the pattern is not followed by the current position.
    - `(?<=pattern)`: Positive lookbehind, matches if the pattern is preceded by the current position.
    - `(?<!pattern)`: Negative lookbehind, matches if the pattern is not preceded by the current position.

9. **Examples:**
    - `re.search(r"cat", "The cat sat on the mat")` will return a match object for "cat".
    - `re.match(r"^cat", "The cat sat on the mat")` will return None since "cat" does not occur at the beginning of the string.
    - `re.findall(r"[aeiou]", "Hello World")` will return a list containing all vowels in "Hello World".
    - `re.search(r"\d{3}-\d{3}-\d{4}", "My phone number is 123-456-7890")` will return a match object for "123-456-7890".
    - `re.findall(r"(red|blue|green)", "I love red, blue, and green colors")` will return a list containing all color names mentioned in the string.



## Basic Regular Expression Operations

1. Importing the `re` module:

```python
import re
```

2. Matching patterns using `re.match()`:

```python
pattern = r"hello"
text = "hello world"
match = re.match(pattern, text)
if match:
    print("Match found!")
else:
    print("No match found.")
```

3. Searching for patterns using `re.search()`:

```python
pattern = r"world"
text = "hello world"
match = re.search(pattern, text)
if match:
    print("Match found!")
else:
    print("No match found.")
```

4. Finding all occurrences of a pattern using `re.findall()`:

```python
pattern = r"o"
text = "hello world"
matches = re.findall(pattern, text)
print(matches)  # Output: ['o', 'o']
```

5. Splitting a string based on a pattern using `re.split()`:

```python
pattern = r"\s+"  # Matches one or more whitespace characters
text = "Hello   World"
split_text = re.split(pattern, text)
print(split_text)  # Output: ['Hello', 'World']
```

6. Replacing patterns in a string using `re.sub()`:

```python
pattern = r"world"
text = "hello world"
new_text = re.sub(pattern, "Python", text)
print(new_text)  # Output: 'hello Python'
```

## Metacharacters and Character Classes

1. Using the `.` (dot) metacharacter to match any character except a newline:

```python
pattern = r"h.t"  # Matches 'hat', 'hot', etc.
text1 = "hat"
text2 = "hot"
match1 = re.match(pattern, text1)
match2 = re.match(pattern, text2)
if match1:
    print("Match found for text1!")
if match2:
    print("Match found for text2!")
```

2. Using the `*` metacharacter to match zero or more occurrences of the preceding character or group:

```python
pattern = r"go*d"  # Matches 'gd', 'god', 'good', etc.
text1 = "gd"
text2 = "good"
match1 = re.match(pattern, text1)
match2 = re.match(pattern, text2)
if match1:
    print("Match found for text1!")
if match2:
    print("Match found for text2!")
```

3. Using character classes to match sets or ranges of characters:

```python
pattern = r"[aeiou]"  # Matches any vowel character
text = "hello"
matches = re.findall(pattern, text)
print(matches)  # Output: ['e', 'o']
```

4. Using anchors to match positions:

```python
pattern = r"^hello"  # Matches 'hello' only if it appears at the start of the string
text1 = "hello world"
text2 = "world hello"
match1 = re.match(pattern, text1)
match2 = re.match(pattern, text2)
if match1:
    print("Match found for text1!")
if match2:
    print("Match found for text2!")
```

5. Using groups and capturing:

```python
pattern = r"(he)(l+o)"  # Matches 'hello' and captures 'he' and 'llo' as groups
text = "hello"
match = re.match(pattern, text)
if match:
    print(match.group(0))  # Output: 'hello'
    print(match.group(1))  # Output: 'he'
    print(match.group(2))  # Output: 'llo'
```

These examples cover some of the basic operations and concepts related to regular expressions in [[Python]]. Regular expressions can be much more complex and powerful, allowing you to handle complex pattern matching scenarios efficiently.


