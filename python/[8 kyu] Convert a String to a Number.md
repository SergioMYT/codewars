# [8 kyu] Convert a String to a Number

---

#### [https://www.codewars.com/kata/544675c6f971f7399a000e79](https://www.codewars.com/kata/544675c6f971f7399a000e79)

## Description

We need a function that can transform a string into a number. What ways of achieving this do you know?

Note: Don't worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.

## Examples

    "1234" --> 1234
    "605"  --> 605
    "1405" --> 1405
    "-7" --> -7

---

## Solution

**Notes**

The `int()` function converts the specified value into an integer number.

    Syntax: int(value, base) 

    - value A number or a string (0-9) that can be converted into an integer  number
    - base 	A number representing the number format. Default value: 10

**Code**

<details>
	<summary>Spoiler</summary>

    def string_to_number(s):
        return int(s)

</details>