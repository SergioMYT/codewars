# [8 kyu] Opposite number

---

#### [https://www.codewars.com/kata/56dec885c54a926dcd001095](https://www.codewars.com/kata/56dec885c54a926dcd001095)

## Description

Given an integer or a floating-point number, find its opposite.

## Examples

    1: -1
    14: -14
    -34: 34

---

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

    def opposite(number):
        return abs(number) if number < 0 else -abs(number)  

</details>

  