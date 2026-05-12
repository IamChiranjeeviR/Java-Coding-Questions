# Investment Share Management System

## Description

### Objective:

To work with classes and objects, and the `static` modifier.

---

# Concept Explanation

A class is a blueprint or template for creating objects.

It defines:

- Attributes (data members)
- Methods (functions)

An object is an instance of a class that contains actual values.

Encapsulation is the concept of bundling:

- Data
- Methods operating on the data

within a single unit called a class.

The `static` modifier is used for variables or methods that belong to the class rather than individual objects.

---

# Concept Implementation

The `Investment` class represents an investment in a company's shares.

It stores:

- Company ID
- Company Name
- Total available shares
- Value of one share

The class includes:

- Getter and Setter methods
- Validation for number of shares
- A method to calculate the total investment amount

The `UserInterface` class:

- Gets input from the user
- Creates Investment objects
- Checks share availability
- Calculates investment amount
- Displays the output

---

# Scenario

Create a class `Investment` with the following private variables:

| Attribute       | Type       |
| --------------- | ---------- |
| companyId       | int        |
| companyName     | String     |
| noOfShares      | static int |
| valueOfOneShare | double     |

---

# Requirements

## Getter and Setter Methods

Include:

- Getters
- Setters

for all attributes.

Getter and Setter names should match the attribute names.

---

# Validation Rule

The variable `noOfShares` should contain only positive integer values.

- Zero is not allowed
- Negative values are not allowed

This validation should be done inside the setter method.

---

# Method Specification

```java
public double calculateTotalAmountOfInvestment(int sharesBought)
```

---

# Method Responsibilities

This method should:

1. Check the availability of shares
2. If shares are available:
   - Reduce `sharesBought` from `noOfShares`
   - Calculate total investment amount

```text
sharesBought × valueOfOneShare
```

3. Round the result to one decimal place
4. Return the total amount

---

# Condition

If shares are not available:

- Return `-1`
- Display:

```text
Shares not available
```

and terminate the program.

---

# UserInterface Class

Write the `main()` method in the `UserInterface` class to test the application.

The program should:

1. Get input from the user
2. Create objects
3. Calculate investment amount
4. Display the result

---

# Note

- Follow the exact class names, attribute names, and method names specified.
- All attributes should be declared as `private`.
- Do not use `System.exit(0)`.
- Follow object-oriented programming standards.

---

# Sample Input / Output flow 1

```text
Enter the number of company shares you bought
2

Enter total number of shares
150

#1st company
Enter the company id
118

Enter the company name
ASSER

Enter the number of shares you bought
100

Enter the value of one share
2000

# Output
Total number of shares=150
Total amount of investment=200000.0
Remaining Available shares=50


# 2nd company
Enter the company id
119

Enter the company name
BOWX

Enter the number of shares you bought
20

Enter the value of one share
10000

# Output
Total number of shares=50
Total amount of investment=200000.0
Remaining Available shares=30

```

# Sample Input / Output Flow 2

```text

Enter the number of company shares you bought
2

Enter total number of shares
25

#1st company
Enter the company id
111

Enter the company name
RRDS

Enter the number of shares you bought
5

Enter the value of one share
1000

# Output
Total number of shares=25
Total amount of investment=5000.0
Remaining Available shares=20


# 2nd company
Enter the company id
112

Enter the company name
YEBS

Enter the number of shares you bought
25

Enter the value of one share
2000

# Output
Shares not available
```
