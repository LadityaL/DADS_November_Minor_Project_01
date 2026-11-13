# Python Fundamentals and NumPy Foundations
## Week 1 Minor Project — The Unlox Academy

**Student:** Aditya Kumar  
**Programme:** Data Science and Data Analytics

## Project Overview

This project covers 50 questions on Python fundamentals and introductory NumPy operations. The work is organised into three Jupyter notebooks covering conceptual explanations, output prediction and practical programming exercises.

## Project Files

| File | Questions | Contents |
| --- | --- | --- |
| `SectionA_Aditya_Kumar.ipynb` | Q1–Q10 | Object identity, mutability, floating-point arithmetic, collections, operators and NumPy fundamentals |
| `SectionB_Aditya_Kumar.ipynb` | Q11–Q15 | Expected outputs, executable examples and explanations of Python behaviour |
| `SectionC_Aditya_Kumar.ipynb` | Q16–Q50 | Calculations, conditionals, patterns, loops, collections, strings, functions and NumPy operations |
| `README.md` | — | Project overview, setup instructions and implementation notes |

Questions appear as headings, with answers and explanations under smaller headings. Code cells include saved demonstration outputs where applicable.

## Requirements

- Python 3
- Jupyter Notebook or Google Colab
- NumPy for Q48–Q50

Only NumPy is imported by the assignment solutions. The remaining exercises use Python's built-in features.

## Running the Notebooks

### Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload the required `.ipynb` file.
3. Run individual code cells using the play button or **Shift+Enter**.
4. Enter the requested values when an input prompt appears.

### Local Jupyter Notebook

Install the notebook application and NumPy:

```bash
python -m pip install notebook numpy
```

Open a terminal in the project folder and start Jupyter:

```bash
python -m notebook
```

Select the required notebook and run its cells in order. Section A contains Markdown explanations and does not require execution. Each Section C solution can also run independently.

## Section B: Expected Exceptions

Two examples intentionally raise exceptions as part of the questions:

- **Q13:** `print(j)` raises `NameError` when `j` has not previously been defined, because the loop over `range(0)` never executes. Use a fresh kernel or runtime to reproduce this result.
- **Q14:** `print("10" + 20)` raises `TypeError`. Execution stops before the last statement in that cell. A separate cell demonstrates the last statement independently.

If **Run All** stops at either exception, continue with the subsequent cells individually. Expected-output sections accompany the code; saved outputs show demonstration runs.

## Section C: Inputs and Behaviour

Input-based exercises prompt for values when executed. Saved outputs show the sample inputs used in demonstration runs. Numeric exercises expect valid numeric text unless input parsing or validation is explicitly included in the solution.

For **Q39**, the state-and-capital menu continues until option **6** is selected.

## Implementation Notes

| Question | Interpretation or behaviour |
| --- | --- |
| Q17 | The delivery threshold is checked against the subtotal before GST, matching the supplied example: ₹450 subtotal + ₹81 GST + ₹40 delivery = ₹571. |
| Q21, Q23 | Tax slabs and electricity rates are implemented as supplied in the assignment. Q21 does not add deductions, rebates, cess or surcharge. |
| Q25 | The assignment's BMI categories are applied to the unrounded result using thresholds of 18.5, 23, 25 and 30. |
| Q27 | The number diamond accepts positive integer sizes and uses loop-based padding to align multi-digit values. |
| Q36 | Words are whitespace-separated tokens. Vowels and consonants use English letters. Spaces are literal spaces; other characters, including tabs, count as special characters. |
| Q37 | Second highest means the second-highest distinct mark. If all marks are equal, no second distinct mark exists. |
| Q38 | Punctuation separates words. Tied word frequencies retain first-appearance order. |
| Q40, Q42 | Set display order may vary between runs without changing the results. |
| Q43 | An empty cleaned sequence is treated as a palindrome. |
| Q44, Q45 | The title-case example assumes words begin with letters; Caesar shifts apply to English uppercase and lowercase letters. |
| Q48 | The diagonal and full-array sums refer to the matrix after scaling by 10; both sums are 50. |

## Validation

All 35 Section C solutions were executed with demonstration inputs. An additional set of 75 sample and edge-case checks covered calculation boundaries, zero inputs, duplicate marks, input parsing, string handling and function results.

Checks also confirmed that:

- The three notebooks contain headings for all 50 questions.
- Q16–Q47 do not import external libraries.
- Section C uses no comprehensions or lambda expressions.
- Q49 and Q50 contain no explicit loops.

The two Section B exceptions described above are expected outputs of the supplied examples.
