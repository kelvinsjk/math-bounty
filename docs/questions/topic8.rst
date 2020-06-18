Topic 8: Integration techniques
==========================================

Question 0801
--------------------------------

The question
^^^^^^^^^^^^^

This question is inspired by the 2008 H2 Mathematics (9740) Paper 1 Question 5.

..  admonition::    Question example

    (a) 
    
        (3 marks) Find the exact value of $\displaystyle \int_0^C \frac{1}{A^2 \pm C^2x^2} \; \mathrm{d}x$.

    (b)
    
        (4 marks) Find the exact value of $\displaystyle \int_1^\mathrm{e} x^{n-1} \ln x \; \mathrm{d}x$ (or $\displaystyle \int_0^1 x \mathrm{e}^{nx} \; \mathrm{d}x$).


Randomly generated elements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
*   :math:`A,B` (9*8 options). 
*   (a) Plus or minus in the denominator (2 options)
*   $C$ (3 options)
*   (b) Choice of integral type (2 options).
*   $n$ (16 options).

This gives the potential for up to 13,824 unique questions.

Pedagogy notes
^^^^^^^^^^^^^^^
We work on numeracy by varying :math:`A,B,C` and :math:`N`.

We work on structure by varying the integrals. For (a), having a plus sign means applying the tangent inverse formula while a minus sign will mean applying the logarithm formula (or using partial fractions).

For (b), the logarithm integral involves differentiating ln and integrating $x^{n-1}$ for our by parts technique. Meanwhile, the exponential integral involves differentiating $x$ and integrating the exponential.

Developer/mathematical notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

For (b), the limits and exponents are chosen such that they will give us the same answer of $\frac{n-1}{n}\mathrm{e}^n + \frac{1}{n^2}$ regardless of the question type.