# Water Tank Capacity Calculator

## Description

### Objective:

To work with control structures.

---

## Concept Explanation

Control structures in Java regulate the flow of execution in a program. This includes conditional statements like `if`, `else-if`, and `switch`, which direct the program flow based on certain conditions. These control structures determine the logic and behaviour of Java programs, allowing for decision-making to achieve desired outcomes.

---

## Concept Implementation

A conditional statement `if` is used to check if the entered radius or height is less than or equal to zero. If so, it prints `"Invalid measurement"`.

Otherwise:

- The total volume of the tank is calculated using the formula for the volume of a cylinder.
- The capacity for the alarm is calculated as `3/4th` of the total capacity.

For output formatting, the `printf` method is used to print the output with 2 decimal places.

```java
System.out.printf("%.2f", value);
```

---

## Scenario

Mr. Smith wants to reduce water waste while filling his water tank. He wants to set an alarm when three-fourths of the tank is filled.

Write a Java program to calculate:

- The total capacity of the tank
- The capacity at which the alarm should ring

Assume that:

- The tank is cylindrical
- The tank is filled only if it is completely drained

Get the radius and height from the user.

Use the formula:

```text
Volume of cylinder = Pi × radius × radius × height
```

If the radius or height is less than or equal to zero, print:

```text
Invalid measurement
```

Otherwise:

- Calculate the total capacity
- Calculate the alarm capacity as `3/4th` of the total capacity
- Print the output with 2 decimal places

---

## Note

- Use Pi value as `3.14`
- Follow the class, attribute, and method names exactly as specified.
- Do not use `System.exit(0);`

---

# Sample Input 1

```text
Enter the radius
28

Enter the height
42
```

# Sample Output 1

```text
Total capacity is 103393.92 litres

Capacity for alarm is 77545.44 litres
```

---

# Sample Input 2

```text
Enter the radius
0

Enter the height
25
```

# Sample Output 2

```text
Invalid measurement
```
