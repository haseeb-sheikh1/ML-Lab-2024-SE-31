# CS-3105 Machine Learning Lab

## Lab 01: Introduction to Python Programming

**Name:** Sheikh Haseeb-ur-Rehman
**Roll No:** 2024-SE-31
**Notebook:** `Lab01_2024-SE-31_Sheikh_Haseeb-ur-Rehman.ipynb`

---

## Overview

This lab covers the basics of Python: arithmetic operators, string methods, string formatting, indexing into nested lists and dictionaries, functions, conditionals, and a few bonus problems using slicing and `max()` with a key function.

## Requirements

- Python 3.9 or higher
- Jupyter Notebook, JupyterLab, or Google Colab

No external libraries are needed. The bonus section only uses the built-in `string` module.

## How to Run

```bash
jupyter notebook Lab01_2024-SE-31_Sheikh_Haseeb-ur-Rehman.ipynb
```

Then run all cells in order (**Kernel → Restart & Run All**). Alternatively, upload the notebook to Google Colab and use **Runtime → Run all**.

---

## Tasks and Expected Output

| Task | Description | Approach | Expected Output |
|------|-------------|----------|-----------------|
| 01 | Calculate 7 to the power of 4 | `**` operator | `2401` |
| 02 | Split `"Hi there Sam!"` into words | `str.split()` | `['Hi', 'there', 'Sam!']` |
| 03 | Print a planet's diameter | `str.format()` | `The diameter of Earth is 12742 kilometers.` |
| 04 | Grab `"hello"` from a nested list | Chained indexing `lst[3][1][2][0]` | `hello` |
| 05 | Grab `"hello"` from a nested dictionary | Mixed keys and indexes `d["k1"][3]["tricky"][3]["target"][3]` | `hello` |
| 06 | List vs. tuple (written answer) | Explanation in markdown | Lists are mutable; tuples are immutable |
| 07 | Extract the domain from an email | `email.split("@")[-1]` | `domain.com` |
| 08 | Check whether `"dog"` is in a string (case-insensitive) | `"dog" in s.lower()` | `True` |
| 09 | Count occurrences of `"dog"` (case-insensitive) | `s.lower().count("dog")` | `2` |
| 10 | Speeding ticket calculator | `if / elif / else` with a birthday adjustment | `Small Ticket` (81, True) and `Big Ticket` (81, False) |

### Task 06: List vs. Tuple

- **List** `[1, 2]` is mutable, so elements can be added, removed, or changed after creation.
- **Tuple** `(1, 2)` is immutable, so its contents are fixed once created.

### Task 10: Speeding Ticket Rules

| Speed | Result |
|-------|--------|
| 60 or less | No Ticket |
| 61 to 80 | Small Ticket |
| 81 or more | Big Ticket |

On your birthday, the speed limits shift by 5 (the speed is reduced by 5 before checking).

---

## Bonus Challenges

| Bonus | Description | Approach | Expected Output |
|-------|-------------|----------|-----------------|
| 1 | `count_dog` that handles punctuation | Strip punctuation with `str.translate`, then count whole words | `2` for `"dog, DOG! dogma"` (`dogma` is not counted) |
| 2 | Palindrome check | Slicing with `w[::-1]` | `True` for `"Racecar"` |
| 3 | Find the top student | `max()` with a `lambda` key on `score` | `Zoe` |

---

## Concepts Practiced

- Arithmetic operators
- String methods: `split()`, `lower()`, `count()`, `translate()`
- String formatting with `.format()`
- Indexing nested lists and dictionaries
- Mutable vs. immutable types
- Defining functions and returning values
- Conditional logic (`if / elif / else`)
- Slicing (`[::-1]`)
- `max()` with `lambda`
