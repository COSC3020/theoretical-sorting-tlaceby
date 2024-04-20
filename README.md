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

**Verifying The Claim**

1. Generate a large set of test cases with varying input sizes (n) and different characteristics. Some tests would provide an input which is already sorted, some being in partial sorted, reverse sorted and obviously random distributions.

2. Measure the execution time of the sorting algorithm for each test case using the black-box.

3. Plot the time against the input size on a graph.

If the claim is true and the sorting algorithm indeed has an $O(n)$ time complexity, I would expect to see a linear relationship between the execution time and the input size. However, if the claim is false I would expect a non-linear growth in the execution time as the input size increases. The execution time would grow faster than the input size.

By conducting this analysis with a sufficiently large and diverse set of inputs it would be clear whether this researcher is lying or not.

**Theoretical Argument**

The lower bound for any comparison based sorting algorithm is $\Omega(n \log n)$. Since our researcher is claiming that his algorithm is $O(n)$ while also using comparison based approach, this cannot be possible given the proven lower bound for any comparison based algorithm is $\Omega(n \log n)$.

# Resources

I was trying to come up with a **proof** for this and could not on my own. However I figured it was important that this researcher said his proprietary algorithm was based on comparing two elements at a time. I searched if there was an already estanblished proof or lower bound for comparison based sorting and indeed there is:

https://www.geeksforgeeks.org/lower-bound-on-comparison-based-sorting-algorithms/
