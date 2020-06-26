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

Licensing
--------------

Math Atlas is developed as an open source project. The underlying code is licensed under the GNU General Public License
v3.0 (`Link to GNU GPL v3.0 <https://choosealicense.com/licenses/gpl-3.0/>`_).

Many of the questions are heavily influenced by old examination questions at the Singapore-Cambridge GCE A Level H2 Mathematics syllabus
(in version 1.0 we have mainly referenced the 2007 and 2008 papers). No copyright is claimed for those questions and they remain the copyright of UCLES and MOE.

The remaining content (newly created questions and the implementation of randomly generated elements) is licensed under
the Creative Commons Attribution-NonCommercial-ShareAlike license (`CC BY-NC-SA <https://creativecommons.org/licenses/by-nc-sa/4.0/>`_).

Fair use
^^^^^^^^^^^^^^^^^^^^^^^^^^

A lot of thought has been put into the types of questions we implement for this application. Past examination questions are often one of the best
tools for students' practice.

We assert that our use of questions from the 2007/2008 papers constitute fair use based on the following:

The transformative factor
~~~~~~~~~~~~~~~~~~~~~~~~~~

We argue that our work in introducing randomly generated elements into the questions, in addition to structuring it as a mobile/web application
(including letting students input their answers and grading them after the attempt) is transformative. This documentation captures some of the
analysis and commentary of the questions in how the random elements are generated.

The nature of the copyrighted work
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It is often a fine line separating the non-copyrightable mathematical idea from the original and creative arrangement of a examination question. 
We have weighed the pros and cons of crafting entirely new questions without reference vs modifying the originals and feel that the added educational
benefit outweights the potential legal ambiguity. We feel that the public (students learning the subject/preparing for their exams) have much to benefit
from repeated practice of past exam questions (vs a static crafted question).

The amount and substantiality of the portion taken
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

While we have modified quite a substantial proportion of the 2007 examination, we argue that it should be taken in the context of all the examination question 
throughout the years (more than 13 years worth of questions from 2007-present for the H2 Mathematics syllabus and subsequent revisions).

The effect of the use upon the potential market
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Past examination questions are most commonly sold as a "ten-year-series" (TYS) featuring the latest 10 years of examination questions. The questions modified in the application
is past this 10 years "window". In fact, we actually recommend students purchase the latest TYS for their learning and examination preparation so we contend that our application
has minimal (or may even have some slight positive) impact on the potential market.

Concluding remarks
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

While we have laid out our arguments of fair use, if you are the copyright owner and believe material has been used in an unauthorized manner, please contact us.

We have modeled our fair use argument based on `this article by Rich Stim. <https://fairuse.stanford.edu/overview/fair-use/four-factors/>`_