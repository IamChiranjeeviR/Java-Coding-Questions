# Fitness Bootcamp Registration System

## Problem Description

A fitness center is organizing a bootcamp program and wants to manage participant registrations efficiently.

Each participant provides the following details:

- Participant Name
- Age
- Fitness Level (`Beginner`, `Intermediate`, or `Advanced`)
- Registration Fee

Your task is to:

1. Store the details of all participants.
2. Count the number of participants in each fitness level category.
3. Calculate the total registration fee collected.
4. Display the participant details along with summary information.

---

## Input Format

- The first line contains an integer `n`, representing the number of participants.
- The next `n` lines contain participant details in the following format:

```text id="k3j8dw"
name age fitnessLevel fee
```

Example:

```text id="s9d2lm"
John 25 Beginner 1500
```

---

## Output Format

- Display the participant details in the same order.
- Then display:
  - Total number of `Beginner`, `Intermediate`, and `Advanced` participants.
  - Total registration fee collected.

---

## Constraints

- `1 ≤ n ≤ 100`
- `18 ≤ age ≤ 60`
- `Fee ≥ 0`

---

## Sample Input

```text id="m7p4zc"
3
John 25 Beginner 1500
Alice 30 Intermediate 2000
Bob 28 Beginner 1500
```

---

## Sample Output

```text id="q8v2nx"
Participant Details:
John 25 Beginner 1500
Alice 30 Intermediate 2000
Bob 28 Beginner 1500

Beginner: 2
Intermediate: 1
Advanced: 0
Total Fee: 5000
```

---

## Explanation

- Participants are categorized based on their fitness level.
- Count each category:
  - Beginner → `2`
  - Intermediate → `1`
  - Advanced → `0`

- Total fee = `1500 + 2000 + 1500 = 5000`

---

## Instructions

- Write a Java program to solve the above problem.
- Use appropriate classes and methods.
- Follow proper input/output formatting as shown in the sample output.

---

## Hint

- Use a class `Participant` to store participant details.
- Use loops to process input and compute counts.
