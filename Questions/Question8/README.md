# Gym Membership Management

## Problem Description

A gym wants to manage its membership records efficiently.

Each member registers with the following details:

- Member ID
- Member Name
- Membership Type (`Basic`, `Standard`, or `Premium`)
- Monthly Fee

Your task is to:

1. Store details of all gym members.
2. Display all member details.
3. Calculate the total monthly revenue generated from all memberships.
4. Identify and display the number of members under each membership type.

---

## Input Format

- The first line contains an integer `n`, representing the number of members.
- The next `n` lines contain member details in the following format:

```text id="m4k9zx"
memberId name membershipType fee
```

Example:

```text id="v7p2qa"
101 Rahul Premium 3000
```

---

## Output Format

- Display the member details in the same order.
- Then display:
  - Number of members in each category (`Basic`, `Standard`, `Premium`)
  - Total monthly revenue

---

## Constraints

- `1 ≤ n ≤ 100`
- Member ID is a positive integer
- `Fee ≥ 0`

---

## Sample Input

```text id="t8n5wr"
3
101 Rahul Premium 3000
102 Anjali Basic 1000
103 Kiran Standard 2000
```

---

## Sample Output

```text id="c3x7lm"
Member Details:
101 Rahul Premium 3000
102 Anjali Basic 1000
103 Kiran Standard 2000

Basic: 1
Standard: 1
Premium: 1
Total Revenue: 6000
```

---

## Explanation

- Members are categorized based on membership type.
- Count:
  - Basic → `1`
  - Standard → `1`
  - Premium → `1`

- Total revenue = `3000 + 1000 + 2000 = 6000`

---

## Instructions

- Write a Java program to solve the above problem.
- Use appropriate classes and methods.
- Follow the exact input/output format.

---

## Hint

- Create a class `Member` with required attributes.
- Use loops to process input and accumulate totals.
