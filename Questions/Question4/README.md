# Restaurant Bill Generation System

## Description

### Objective:

To work with classes and objects.

---

# Concept Explanation

Classes and objects are fundamental concepts in object-oriented programming.

- **Class** acts as a blueprint or template for creating objects.
- **Object** is an instance of a class.

A class defines:

- Attributes (data members)
- Methods (behaviors)

Objects contain their own data and can perform operations defined in the class methods.

---

# Concept Implementation

The `Restaurant` class is designed to represent a restaurant order.

It stores:

- Customer name
- Order number
- Delivery type
- Food name
- Phone number

The class also provides a method to calculate the total bill amount based on:

- Food cost
- Delivery type

The `UserInterface` class:

- Gets input from the user
- Creates the `Restaurant` object
- Validates the delivery type
- Displays the bill details

---

# Scenario

Brilliant Restaurant is a newly started restaurant.

They provide:

- Home delivery
- Parcel service
- Normal orders

The restaurant wants to automate the bill generation process based on the order type.

Develop a Java application to:

- Store order details
- Calculate the bill amount
- Display the final bill

---

# Component Specification: Restaurant Class

| Attribute    | Type   |
| ------------ | ------ |
| customerName | String |
| orderNumber  | int    |
| deliveryType | String |
| foodName     | String |
| phoneNumber  | long   |

---

## Requirements

### Constructor

Include a **public parameterized constructor** with the following arguments in order:

```text
customerName, orderNumber, deliveryType, foodName, phoneNumber
```

---

## Getter and Setter Methods

Include:

- Getters
- Setters

for all attributes.

---

# Method Specification

| Component Name       | Class      | Method                                          | Responsibility                             |
| -------------------- | ---------- | ----------------------------------------------- | ------------------------------------------ |
| Calculate total bill | Restaurant | `public double calculateTotalBill(double cost)` | Calculate and return the total bill amount |

---

# Formula for Bill Calculation

```text
Bill Amount = (Cost × Tax) + Cost
```

---

# Delivery Type and Tax

| Delivery Type | Tax |
| ------------- | --- |
| HomeDelivery  | 0.8 |
| Parcel        | 0.5 |
| NormalOrder   | 0.3 |

---

# Example

If:

```text
Cost = 18
DeliveryType = NormalOrder
```

Then:

```text
Bill Amount = (18 × 0.3) + 18
Bill Amount = 5.4 + 18
Bill Amount = 23.4
```

---

# UserInterface Class

Write the `main` method in the `UserInterface` class.

The program should:

1. Get input from the user
2. Validate delivery type
3. Create the Restaurant object
4. Calculate the bill
5. Display the output

---

# Validation Rule

If the `deliveryType` is not one of:

```text
HomeDelivery
Parcel
NormalOrder
```

then print:

```text
Invalid Order Type
```

and terminate the program.

---

# Note

- The `deliveryType` is case-sensitive.
- All attributes should be declared as `private`.
- All classes and methods should be declared as `public`.
- Follow the exact class names, attribute names, and method names specified.
- Do not use `System.exit(0)`.

---

# Sample Input 1

```text
Enter the Name
Alfred

Enter the Order Number
3343

Enter the Delivery Type
NormalOrder

Enter the Food Name
ChickenBurger

Enter the Phone Number
8899889977

Enter the price of the item
18
```

---

# Sample Output 1

```text
Name Alfred

Order Number 3343

Delivery Type NormalOrder

Food Name ChickenBurger

Phone Number 8899889977

Bill Amount 23.4
```

---

# Sample Input 2

```text
Enter the Name
James

Enter the Order Number
43433

Enter the Delivery Type
OnlineOrder
```

---

# Sample Output 2

```text
Invalid Order Type
```
