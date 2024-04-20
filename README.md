[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/9YUeXH71)

# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

## Solution

**IDEAS:**

Generate large test data and compare it to what you would expect. Since the algorithm is supposed to be $O(n)$, this would mean that on average the expected results would all be linear for a certain dataset.

- Create test data, (sorted, random shuffles, partially sorted, etc...)
- Run it through this black box and gather some data.
  - Execution time should average a linear trend with the size of the input.
  - If it's not statistically consistent with a linear approximation then this would mean the algorithm is indeed not acttually $O(n)$.

**THEORETICAL:**
WTF??
