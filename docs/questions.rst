Questions
=========

Topic 5: the sigma notation
--------------------------------

Question 0501
^^^^^^^^^^^^^

The question
~~~~~~~~~~~~

This question is inspired by the 2007 H2 Mathematics (9740) Paper 2 Question 2.

..  admonition::    Question example

    Let :math:`\displaystyle u_n=\frac{n-1}{n}`

    (a)     
    
        (i) (2 marks) Prove that :math:`\displaystyle u_{n+1}-u_{n}=\frac{1}{n(n+1)}`
        (ii) (2 marks) Hence find :math:`\displaystyle \sum_{n=1}^N \frac{1}{n(n+1)}`
        (iii)  (3 marks) Give a reason why the series in (aii) is convergent and state the sum to infinity.

    (b) (2 marks) Use your answer to part (aii) to find :math:`\displaystyle \sum_{n=2}^N \frac{1}{n(n-1)}`

Randomly generated elements
~~~~~~~~~~~~~~~~~~~~~~~~~~~
*   :math:`u_n` can be of the form :math:`\frac{1}{n^2},\frac{1}{n},\frac{n-1}{n},\frac{n}{n+1},\frac{n+1}{n},` or :math:`\frac{n}{n-1}`. (6 options)
*   In (ai), the question could ask for a difference between :math:`u_n` and (:math:`u_{n-1}` or :math:`u_{n+1}`) in either order. (4 options)
*   In (aii), the bottom limit could be a number from 1 to 5 (checking to make sure such a limit is valid). (5 options)
*   In (b), we could replace :math:`n` with :math:`n\pm 1` or :math:`n\pm 2`. (4 options)

This gives the potential for up to 480 unique questions.

Pedagogy notes
~~~~~~~~~~~~~~
The variation in numbers/algebraic terms is achieved with modifiying :math:`u_n`.

The variation in the structure of the question comes from changing the order of the difference :math:`u_{n+1}-u_{n}`. We will thus see cancelation either down towards the right or down towards the left.

Developer notes
~~~~~~~~~~~~~~~
Unlike most other questions where the variables used to randomly generated question are usually self-explanatory (they either directly describe the variable or is simply an arbitrary placeholder), the creation of :math:`u_n` uses a certain non-intuitive structure so that we could easily extend the randomly generated elements with just a few modifications.

The main observation is that the numerator or denominator of :math:`u_n` are usually of the form :math:`n,n-1` or :math:`n+1`. During (ai), we could potentially end up with terms such as :math:`n-2` or :math:`n+2` as well. The odd one out out of the 6 options listed above is the number 1 (considering squares can be easily appended). The terms in this question will often be modified with :math:`n\pm 1` so they shift up or down a 'chain' of the form :math:`[n-2, n-1, n, n+1, n+2]`, with the exception of the number 1. So we wanted to create a system to keep track of these changes in the term without resorting to symbolic manipulation or extensive cases.

Thus we created the following number system: our elements will be :math:`{0, 2, 4, 8, 16, 32}` where '0' will to assigned to the number 1, '2' assigned to :math:`n-2`, '4' to :math:`n-1`, etc and '32' assigned to :math:`n+2`. To perform operations/substitutions, we multiply/divide by 2. Thus '0' will always stay as 0 while the other terms can be moved up and down the chain. We just have to be careful not to go below '2' or above '10'. If we require more terms in the future like :math:`n\pm 3`, etc, we can simply add more multiples of 2 into our chain to create the same effect.

We think of this as an implementation of the directed graph made up of an isolated vertex along with a path (in both directions) with 5 vertices. The edges are implemented by multiplying or dividing by 2. Further exploration may be interesting to explore whether our implementation confers an advantage compared to the more traditional adjacency list/matrix or incidence matrix.
