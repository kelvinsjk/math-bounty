Topic 9: Definite integrals
==========================================

Question 0901
--------------------------------

The question
^^^^^^^^^^^^^

This question is inspired by the 2007 H2 Mathematics (9740) Paper 2 Question 4(ii).

..  admonition::    Question example

    The region $R$ is bounded by the curve $y=x^2 \sin nx$ (or $y=x^2 \cos nx$ or $y=x^2 \mathrm{e}^{nx}$), the line $x=\frac{1}{2}\pi$ (or $x=\pi$ for the sine case, or $x=\frac{2}{n}$ for the exponential case)
    and part of the $x$-axis between $0$ and $\frac{1}{2}\pi$. Find

    (a) 
    
        (5 marks) Find the exact area of $R$.

    (b)
    
        (2 marks) Find the numerical value of the volume of revolution when $R$ is rotated completely about the $x$-axis, giving your answer correct to 3 decimal places.


Randomly generated elements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
*   :math:`n` (9 options). 
*   Choice of function: sine, cosine or exponential (3 options)
*   For the sine case, a choice of $\pi$ or $\frac{\pi}{2}$ as the upper limit.

This gives the potential for up to 36 unique questions.

Pedagogy notes
^^^^^^^^^^^^^^^
We work on numeracy by varying :math:`n` and the function.

Developer/mathematical notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

For working out the solution to (b), we contemplated using the exact answers from repeated use of integration by parts or implementing a numeric solver into our program. We have gone
with the latter and implemented Simpson's 3/8th rule. Based on testing 100 iterations can comfortably provide us with our required accuracy of 3 decimal places.