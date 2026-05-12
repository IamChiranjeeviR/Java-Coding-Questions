# WordZee - String Validation and Manipulation

## Objective

To work with strings.

---

## Concept Explanation

Strings are sequences of characters used to store and manipulate textual data. In programming languages like Java, strings are treated as objects and provide various methods for operations such as:

- Concatenation
- Comparison
- Searching
- Validation
- Manipulation

Strings are immutable in Java, meaning once a string object is created, its value cannot be changed.

---

## Concept Implementation

- Words and sentences are stored as strings.
- Strings are validated to ensure they contain only alphabetic characters and spaces.
- Words are searched within sentences using string manipulation methods.
- Appropriate error messages are displayed for invalid inputs.

---

## Scenario

**WordZee** is a famous game used to improve children's memory and spelling skills.

The teacher asks children to:

1. Spell a word correctly.
2. Reverse the spelling of the word.

As a Java developer, you need to help the teacher verify the children’s answers.

If the given word exists in the sentence, reverse only that word in the sentence and display the modified sentence.

---

## Constraints

### Sentence Validation

If the sentence contains any:

- Number
- Special character

Display:

```text
<sentence> is an invalid sentence
```

---

### Word Validation

If the word contains any:

- Number
- Special character

Display:

```text
<word> is an invalid word
```

---

### Word Search Validation

If the word is not present in the sentence, display:

```text
<word> is not in the sentence
```

---

## Note

- Follow the object-oriented specifications provided in the question.
- Use the class names, attribute names, and method names exactly as specified.
- Adhere to the code template if provided.
- Do not use `System.exit(0)` to terminate the program.

---

# Sample Input and Output

## Sample Input / Output - 1

### Input

```text
Enter a sentence
He ate a delicious pizza for dinner

Enter a word
ate
```

### Output

```text
He eta a delicious pizza for dinner
```

---

## Sample Input / Output - 2

### Input

```text
Enter a sentence
She is studying diligently for her exams

Enter a word
e1fn
```

### Output

```text
e1fn is an invalid word
```

---

## Sample Input / Output - 3

### Input

```text
Enter a sentence
The cat chased the mouse across the room

Enter a word
phoo
```

### Output

```text
phoo is not in the sentence
```

---

## Sample Input / Output - 4

### Input

```text
Enter a sentence
I like coo9@667
```

### Output

```text
I like coo9@667 is an invalid sentence
```
