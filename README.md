# Lab07
# Number Theory: Subtraction


In this lab you've learned the basics of number theory as it relates to subtraction.


## Rubric


| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |


## Names
Group 7: Aaron Ray and Draegan Carley

## Summary
This week we learned how to use logic gates and our full_adder from the previous lab to subtract binary numbers. We started by creating a half subtractor, which was similar to our half adder but used a borrow instead of a carry. We then learned how to use One's Complement and Two's Complement to represent negative numbers and perform subtraction using circuits. I think this lab helped us better understand how we can use the same basic circuits for both addition and subtraction.

## Lab Questions

### 1 - Explain the differences between our Half Adder from the last lab and the Half Subtractor from this lab.
The main difference is that the half adder uses an AND gate to determine the carry out, while the half subtractor uses a NOT gate on A and an AND gate to determine if a borrow is needed. The half adder adds two bits together, while the half subtractor subtracts B from A.


### 2 - What about the end around carry of One’s Complement makes it hard to use and implement?
The end around carry makes One's Complement harder to implement because when there is a carry out of the last bit, we have to take that carry and add it back to the first bit. This means we cannot just connect the full adders together like we did in the previous lab. We need additional circuitry to handle the carry without creating a combinational loop. This makes the circuit more complicated than normal binary addition.


### 3 - What is the edge case and problem with Two’s Complement number representation?
The problem with Two's Complement is that it has one more negative number than positive numbers that it can represent. For example, with 8 bits we can represent numbers from -128 to +127. This means that if we try to find the Two's Complement of -128, we cannot represent the positive 128 because it is outside the range. Instead, the result stays -128 due to overflow. This is an edge case we have to be aware of when working with Two's Complement numbers.
