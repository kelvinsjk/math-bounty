Topic 7: Maclaurin series
==========================================

Question 0701
--------------------------------

The question
^^^^^^^^^^^^^

This question is inspired by the 2008 H2 Mathematics (9740) Paper 1 Question 6a.

..  admonition::    Question example

    In a triangle $ABC$, $BC=a$, angle $BCA = \theta$ radians and $CA=b$ (or angle $CBA=\alpha$). Given that $\theta$ is a sufficiently small angle, show that

    (a) 
    
        (2 marks) $AB \approx (A+B\theta^2)^{\frac{1}{2}}$ (or $A'\sqrt{B'}\theta$).

    (b)
    
        (3 marks) Hence show that $AB \approx C+D\theta^2$ (or $(A+AB^2)^{\frac{1}{2}} \approx C+D\theta^2$).


Randomly generated elements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
*   :math:`a,b` (${13 c\choose 2} - 5 = 73$ options). We choose $a,b$ such that $ab$ is not a perfect square.
*   We either give the student two sides and one angle, or one side and two angles (2 options).
*   For the two angles case, either $\alpha = \frac{\pi}{4}$ or $\frac{\pi}{3}$ (2 options).

This gives the potential for up to 99 unique questions.

Pedagogy notes
^^^^^^^^^^^^^^^
We work on numeracy by varying :math:`a,b` and :math:`\alpha`.

We work on structure by either giving the student two sides and an angle or one side and two angles. In the first case we will be using the cosine rule and the cosine Maclaurin series while for the second case we will be using the sine rule and the sine Maclaurin series.

Developer/mathematical notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

For the question to not get too complicated (no surds during the binomial expansion step in (b) we need to generate $a,b$ such that $a,b$ is not a perfect square. The probability of the
complement is closely related to the prime number theorem with an asymptotic probability of $C\frac{\log n}{n} + \frac{A}{n} + O(n^{-\frac{4}{3}}$. See `Noam D. Elkies' solution to this question on mathoverflow <https://mathoverflow.net/questions/279127/probability-that-product-is-a-perfect-square>`.

We have also written a "surd simplify" function to simplify surds of the form $\sqrt{n}$ into the simplified expression $a \sqrt{b}$. Doing such a simplification is essentially the famous prime factorization problem we encounter in the P vs NP problem and in RSA cryptography. Thankfully, we are dealing with small numbers so we have simply implemented a trial division algorithm.