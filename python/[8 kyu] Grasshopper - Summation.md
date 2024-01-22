# [8 kyu] Grasshopper - Summation

---

#### [https://www.codewars.com/kata/55d24f55d7dd296eb9000030](https://www.codewars.com/kata/55d24f55d7dd296eb9000030)

## Description

Write a program that finds the summation of every number from 1 to num. The number will always be a positive integer greater than 0.

## Examples

    2 = 3 (1 + 2)
    8 = 36 (1 + 2 + 3 + 4 + 5 + 6 + 7 + 8)

---

## Solution

**Notes**

The `range()` function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and stops before a specified number.

    Syntax: range(start, stop, step) 

    - start Optional. An integer number specifying at which position to start. Default is 0
    - stop  Required. An integer number specifying at which position to stop (not included).
    - step  Optional. An integer number specifying the incrementation. Default is 

    Example:
        # Create a sequence of numbers from 5 to 9
        x = range(5, 10)

**Code**

<details>
	<summary>Spoiler</summary>

    def summation(num):
        sum = 0
        for n in range(1, num+1):
            sum = sum + n
        return sum
    
</details>

## Solution

**Notes**

The `sum()` function returns a number, the sum of all items in an iterable.

    Syntax: sum(iterable, start)
    
    - iterable 	Required. The sequence to sum
    - start 	Optional. A value that is added to the return value

**Code**

<details>
	<summary>Spoiler</summary>

    def summation(num):
        return sum(range(num+1))
    
</details>