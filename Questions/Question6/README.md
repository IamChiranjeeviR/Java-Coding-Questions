# Sum of Unique Numbers After Doubling Even Elements

## Problem Description

You are given an integer array of size `n`.

Your task is to process the array based on the following rules:

- Double the value of all even numbers in the array.
- Keep the odd numbers unchanged.
- After applying the above transformation, identify all the unique elements in the updated array.
- Calculate and print the sum of these unique elements.

---

## Input Format

- The first line contains an integer `n`, representing the number of elements in the array.
- The second line contains `n` space-separated integers, representing the elements of the array.

---

## Output Format

- Print a single integer representing the sum of unique elements after doubling the even numbers.

---

## Constraints

- `1 ≤ n ≤ 1000`
- `-10^4 ≤ array elements ≤ 10^4`

---

## Sample Input 1

```text
6
1 2 3 2 4 3
```

## Sample Output 1

```text
16
```

## Explanation 1

- Original array: `[1, 2, 3, 2, 4, 3]`
- After doubling even numbers: `[1, 4, 3, 4, 8, 3]`
- Unique elements: `{1, 4, 3, 8}`
- Sum = `1 + 4 + 3 + 8 = 16`

---

## Sample Input 2

```text
5
5 6 7 8 5
```

## Sample Output 2

```text
40
```

## Explanation 2

- Original array: `[5, 6, 7, 8, 5]`
- After doubling even numbers: `[5, 12, 7, 16, 5]`
- Unique elements: `{5, 12, 7, 16}`
- Sum = `5 + 12 + 7 + 16 = 40`
