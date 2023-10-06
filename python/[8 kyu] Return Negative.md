# [8 kyu] Return Negative

---

#### [https://www.codewars.com/kata/55685cd7ad70877c23000102/](https://www.codewars.com/kata/55685cd7ad70877c23000102/)

## Description

In this simple assignment you are given a number and have to make it negative. But maybe the number is already negative?

## Examples

    make_negative(1);  # return -1
    make_negative(-5); # return -5
    make_negative(0);  # return 0

## Notes

- The number can be negative already, in which case no change is required.
- Zero (0) is not checked for any specific sign. Negative zeros make no mathematical sense.

---

## Solution

**Notes**

The `abs()` function returns the absolute value of the specified number.

    Syntax: abs(number)

The symbol `-` is used to change a number from positive to negative or vice versa. It is the same as multiplying a number by minus one.

    Example:
        n = 5
        
        num = n * - 1

        print(num) # return -5

**Code**

<details>
	<summary>Spoiler</summary>

    def make_negative(number):
        return - abs(number)

</details>

---

## Solution

**Notes**

The Python ternary operator determines if a condition is true or false and then returns the appropriate value in accordance with the result. 

    Syntax: 
        [on_true] if [expression] else [on_false] 

    Example:        
        a = 5 
        b = 10
        
        # Assigns the value of a in min if a < b otherwise assigns b
        min = a if a < b else b
 
        print(min) # return 5

**Code**

<details>
	<summary>Spoiler</summary>

    def make_negative(number):
        return number if number <= 0 else - number

</details>