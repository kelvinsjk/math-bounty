Topic 6: differentiation and applications
==========================================

Question 0601
--------------------------------

The question
^^^^^^^^^^^^^

This question is inspired by the 2008 H2 Mathematics (9740) Paper 1 Question 7.

..  admonition::    Question example

    .. image:: qn0601b.svg
        :width: 49%
    .. image:: qn0601a.svg
        :width: 49%

    A plot of land is being designed for a farm. The plot of land consists of a rectangle :math:`x` m by :math:`y` m together with a(n) semicircle/equailateral triangle of diameter/sides semicircle :math:`x` m, as shown in the diagram. Fences will be built along the perimeter of this plot of land. The cost of building the fence along the outside of the rectangle is :math:`\$a` per metre while the cost of building the fence along the outside of the semicircle/triangle is :math:`\$b` per metre. It is given that the total cost of building the fence is :math:`\$k` and the total area of the plot of land is denoted by :math:`A`.

    (a) 
    
        (i) (2/1 marks) Show that :math:`y = f(x)`
        (ii) (2/3 marks) Hence show that :math:`A=g(x)`

    (b)
    
        (i) (4 marks) Use differentiation to find the values of :math:`x` and :math:`y` which gives a stationary value of :math:`A`.
        (ii) (2 marks) Determine, with a reason, whether the values of :math:`x` and :math:`y` in (bi) gives a minimum or maximum value of :math:`A`.

Randomly generated elements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
*   :math:`a,b` and :math:`c` (8*9*19 options)
*   Either a semicircle or a triangle (2 options)

This gives the potential for up to 2736 unique questions.

Pedagogy notes
^^^^^^^^^^^^^^^
We work on numeracy by varying :math:`a,b` and :math:`c`.

We work on structure by modifying the type of figures used. For part (a), either trigonometry or pythagoras theorem has to be used for the triangle while the formulas (circumference and area) for a circle will be tested.  

Developer/mathematical notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

$b$s will be generated such that our answer will be the same up to a substitution of $\pi$ and $\sqrt{3}$.

We are guaranteed a maximum value and valid $x$ and $y$s for this question for all $a,b > 0$ because our two special values, $\pi$ and $\sqrt{3}$ happen to be less than 4. If we ever modify this question to include addtional possibilities in addition to $\pi$ and $\sqrt{3}$ and they happen to be at least 4, we will need further restrictions on $a$ and $b$ (at the moment it seems that $b>\frac{a}{2}$ guarantees a maximum value of $A$ and $x$ positive while $b>a$ guarantees that $y$ will be positive).
