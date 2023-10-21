# Simple Spell Checker for the English Language

## Table of Contents
- [Overview](#overview)
- [How It Works](#how-it-works)
- [Usage](#usage)
- [Example](#example)
- [Authors](#authors)

## Overview

Welcome to our simple spell checker project for the English language. This tool is designed to help you identify and correct misspelled words in your text. It relies on a lexicon (a list of valid words) to make corrections and provide suggestions.

## How It Works

Our spell checker operates based on the following principles:

1. **Text Comparison**: The tool processes text by comparing each word with the words in its lexicon.

2. **Valid Words**: Words that are found in the lexicon are considered correct and do not require correction.

3. **Handling Misspelled Words**: For unrecognized or misspelled words, our spell checker utilizes the "Levenshtein distance" algorithm to find the closest match within the lexicon. The Levenshtein distance measures the similarity between two words by counting the number of single-character edits (insertions, deletions, or substitutions) required to transform one word into another.

4. **Simplified Task**: To streamline the correction process, our spell checker narrows down the search for corrections by comparing incorrect words of length l1 with words of length l2, where l2 is at most two characters longer than l1.

5. **Evaluation**: At the end of the spell checking process, the corrected text is compared with the reference text. Our spell checker then provides two key evaluation metrics:
   - **Recall**: A measure of how many misspelled words were successfully corrected out of the total.
   - **Precision**: A measure of how many of the suggested corrections were accurate out of the total suggestions.

## Usage

1. Clone or download this repository.
2. Prepare your text to be spell-checked (or use the existing file - text.txt).
3. Run the spell checker program (I provided the .ipynb file).
4. Review the corrected text and evaluation metrics (recall and precision).

## Example

To run the spell checker, use the following command (if you download the file in .py format):

```bash
python spell_checker.py
