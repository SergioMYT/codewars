# [6 kyu] Find the odd int

---

#### [https://www.codewars.com/kata/54da5a58ea159efa38000836](https://www.codewars.com/kata/54da5a58ea159efa38000836)

## Description

Given an array of integers, find the one that appears an odd number of times.

There will always be only one integer that appears an odd number of times.

## Examples

    [7] should return 7, because it occurs 1 time (which is odd).
    [0] should return 0, because it occurs 1 time (which is odd).
    [1,1,2] should return 2, because it occurs 1 time (which is odd).
    [0,1,0,1,0] should return 0, because it occurs 3 times (which is odd).
    [1,2,2,3,3,3,4,3,3,3,2,2,1] should return 4, because it appears 1 time (which is odd).

---

## Solution

**Notes**

The modulo `(%)` operation returns the remainder or signed remainder of a division, after one number is divided by another.

In an list, the `count()` method is used to return the number of occurrences of a value or item in an set.

    Syntax: set.count(n)

    - n is the value we want to check for its number of occurrences.

    Example:

    set = [1, 2, 2, 3, 2]
    repeatedNumberTwo = set.count(2)
    print(repeatedNumberTwo) # return 3

**Code**

<details>
	<summary>Spoiler</summary>

    def find_it(seq):
        for n in seq:
            if seq.count(n) % 2 != 0:
                return n 
    
</details>

<details>
	<summary>Spoiler</summary>

    def find_it(seq):
        return [n for n in seq if seq.count(n) % 2 != 0][0] 
    
</details>
