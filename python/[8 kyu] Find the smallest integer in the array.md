# [8 kyu] Find the smallest integer in the array

---

#### [https://www.codewars.com/kata/55a2d7ebe362935a210000b2](https://www.codewars.com/kata/55a2d7ebe362935a210000b2)

## Description

Given an array of integers your solution should find the smallest integer. 

## Examples


- Given `[34, 15, 88, 2]` your solution will return `2`
- Given `[34, -345, -1, 100]` your solution will return `-345`

## Notes

You can assume, for the purpose of this kata, that the supplied array will not be empty.

---

## Solution

**Notes**

The `min()` function returns the item with the lowest value, or the item with the lowest value in an iterable.

If the values are strings, an alphabetically comparison is done.

    One or more items to compare

        Syntax: 
            min(n1, n2, n3, ...)

    An iterable, with one or more items to compare

        Syntax: 
            min(iterable) 

**Code**

<details>
	<summary>Spoiler</summary>

    def findSmallestInt(arr):
        return min(arr) 

</details>