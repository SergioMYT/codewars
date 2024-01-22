# [6 kyu] Find the odd int

---

#### [https://www.codewars.com/kata/546f922b54af40e1e90001da](https://www.codewars.com/kata/546f922b54af40e1e90001da)

## Description

Given a string, replace every letter with its position in the alphabet.
If anything in the text isn't a letter, ignore it and don't return it.

## Examples

    alphabet_position("The sunset sets at twelve o' clock.")

    Should return "20 8 5 19 21 14 19 5 20 19 5 20 19 1 20 20 23 5 12 22 5 15 3 12 15 3 11"

---

## Solution

**Notes**

<details>
	<summary>Explanation</summary>

`[*...]` This is known as "unpacking". We take each character in the string and create a list.

In a String, `lower()` converts all characters to lowercase.

In a String, `find(c)` we use it to find characters within the string

In a String, `index(c)+1` we get the index of the character and add one to the position because the index starts at 0.

</details>

**Code**

<details>
	<summary>Spoiler</summary>

    def alphabet_position(text):
        alphabet = 'abcdefghijklmnopqrstuvwxyz'
        result = '';
    
        for c in [*text.lower()]:
            if (alphabet.find(c) >= 0):
                result = '{} {}'.format(result,str(alphabet.index(c)+1))
        
        return result.strip()
    
</details>