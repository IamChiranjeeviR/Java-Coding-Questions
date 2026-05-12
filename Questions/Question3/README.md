# Whale Fishing Club Points Calculator

## Description

### Objective:

To work with strings.

---

## Concept Explanation

Strings in Java are sequences of characters used to represent text. They are immutable, meaning their content cannot be changed once created.

Strings support various operations such as:

- Concatenation
- Splitting
- Substring extraction
- Comparison
- Parsing values

Strings are widely used for text processing and manipulation in Java programs. Internally, strings are encoded using formats such as ASCII or UTF-8.

In this application, strings are used to:

- Extract participant details from a single input
- Validate age and fish counts
- Calculate fishing competition points

---

## Concept Implementation

The participant details are provided as a single string separated by colons (`:`).

Format:

```text
<participant name>:<participant age>:<big fish>:<medium fish>:<small fish>
```

The program should:

1. Split the string using the `split()` method
2. Extract participant details
3. Validate age
4. Validate fish counts
5. Calculate points based on fish size

### Points System

| Fish Type | Points |
| --------- | ------ |
| Big       | 10     |
| Medium    | 6      |
| Small     | 3      |

---

## Scenario

The Whale Fishing Club (WFC) conducted a fishing competition on a big lake.

Participants:

- Must be 18 years or older
- Catch fish of different sizes
- Earn points based on the size and count of fish caught

Help WFC develop a Java application to calculate the participant's total score.

---

## Requirements

1. Determine points based on fish size:

```text
Big Fish    = 10 points
Medium Fish = 6 points
Small Fish  = 3 points
```

2. Take input from the user as a single string separated by colon (`:`)

```text
<participant name>:<participant age>:<big fish>:<medium fish>:<small fish>
```

3. If age is less than 18, print:

```text
<age> is an invalid age
```

and terminate the application.

4. If any fish count is less than 0, print:

```text
<fish count> is an invalid input
```

and terminate the application.

---

## Note

- Follow the object-oriented specifications provided in the question description.
- Use the class, attribute, and method names exactly as specified.
- Do not use `System.exit(0)` to terminate the program.
- In the sample input/output, the highlighted text represents user input.

---

# Sample Input 1

```text
Enter the details
Hari:20:5:9:15
```

# Sample Output 1

```text
Hari scored 149 points
```

---

## Explanation

```text
Big fish    = 5 × 10 = 50
Medium fish = 9 × 6  = 54
Small fish  = 15 × 3 = 45

Total points = 50 + 54 + 45 = 149
```

---

# Sample Input 2

```text
Enter the details
Quil:15:2:7:2
```

# Sample Output 2

```text
15 is an invalid age
```

---

# Sample Input 3

```text
Enter the details
Allan:22:-1:2:3
```

# Sample Output 3

```text
-1 is an invalid input
```
