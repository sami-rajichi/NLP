# TP1: Basic Text Processing - Regular Expressions and Edit Distance Measurement

## Assignment 1

In this exercise, the goal is to extract email addresses, postal codes, and phone numbers from the "contact us" pages of several Tunisian university websites. To solve this problem, we will use regular expressions.

### Information to be Extracted

#### Phones

There are various formats for phone numbers, for example:
- (216) 73 683 100
- (+216) 73 683 100
- (216) 73683100
- 73683100
- (+216) 73 68 31 00
- 73683100
- etc.

The desired format is: "(+216) XX XX XX XX" where X is a digit.

#### Email Addresses

There are no specific conditions for email addresses.

#### Postal Codes

Postal codes are usually found in institute addresses and typically consist of 4 digits (e.g., 3021).

## How to Use the Code

1. [Download the code](https://github.com/sami-rajichi/NLP/blob/main/RegExp/TP1_EX1.ipynb)
2. Run the main script (Remember to download the HTML files as well).

## Evaluation of the Work

- **Recall**: 0.8823
- **Precision**: 0.9836
- **F1-score**: 0.9302

