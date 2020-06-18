.. Math Bounty documentation master file, created by
   sphinx-quickstart on Thu May 28 23:44:38 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Math Atlas and Math Bounty
======================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   self
   math-atlas
   questions/index

Introduction
----------------------------------------------------------------
We will describe the structure of the documentation here.

Version guide
--------------

Current version: 0.0.1
^^^^^^^^^^^^^^^^^^^^^^^^^^

Added Math Atlas documentation: refer to Math Atlas version guide for more information.


Previous versions
^^^^^^^^^^^^^^^^^^^^^^^^^^

Version 0.0.0
~~~~~~~~~~~~~~

Still in testing phase, nothing functional. 
We plan to move Math Bounty to version 0.1.0 when Math Atlas is ready for release and then to version 1.0.0 when Math Bounty is ready for release.

Developer blog
---------------

Latest: Jun 19, 2020
^^^^^^^^^^^^^^^^^^^^^
We are more than halfway through content generation for Math Atlas. Typescript has been a joy to work with (for the most part) and we're slowly
making our code more and more modular as we progress. The student input/student radio components have really helped our workflow efficiency, and 
better understanding of the onsen-ui page loading/javascript flow process means less messy bugs as we're coding. Now the main bottleneck is in integration testing (and the testing
of the mathematical logic underneath each question). 

At the moment we're aiming to ship with 3 functionalities: an MF26 viewer, question selector by topic as well as a random question selector. 


Previous entries
^^^^^^^^^^^^^^^^^

Jun 1, 2020
^^^^^^^^^^^^^^^^^^^^^
After reading about TypeScript in the latest stackoverflow survey, we have decided to transition to TypeScript ourselves.

May 29, 2020
~~~~~~~~~~~~

Two products are planned: 

1. Math Atlas, a hybrid app featuring 10-14 questions, with an interface for students to key in answers and be graded.
2. Math Bounty, a web app that generates questions into worksheets. 

We have currently coding Math Atlas and plan to port the questions over to Math Bounty after release. We decided to move from a code first approach to a design first approach and will thus be writing documentation for the questions starting from question 5. As of today, that is the only working page in this documentation.


*italics* vs **bold** vs ``this is code``

term
   Definition

.. math::

   (a + b)^2 = a^2 + 2ab + b^2

   (a - b)^2 = a^2 - 2ab + b^2

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
