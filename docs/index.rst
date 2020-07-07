.. Math Bounty documentation master file, created by
   sphinx-quickstart on Thu May 28 23:44:38 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Math Atlas and Math Bounty
======================================

.. toctree::
   :maxdepth: 2

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



Roadmap
--------------

We structure our development roadmap based on our model of the ways student learn. 

Our model of learning
^^^^^^^^^^^^^^^^^^^^^^^^

Medium
~~~~~~~~~

*  Mobile (phone or tablet)
*  Computer (laptop or PC)
*  Physical (paper and/or books)

Phases of learning
~~~~~~~~~~~~~~~~~~~

*  Background: the prerequisites, assumed knowledge and general foundation the student has built up. At the pre-univeristy level the baseline typically involve
   arithmetic (operations involving numbers), algebra (operations on and manipulation of symbols and functions such as polynomials, surds and the trigonometric, logarithmic
   and exponential functions). Some topics may require other specific background knowledge (e.g. coordinate geometry). 

   A strong foundation means that students can channel most of the cognitive load on the acquisition of new concepts. A weaker foundation will mean having to grapple with
   both new and old knowledge simultaneously: this often means the learning process becomes more tiring and the pickup of new knowledge is less efficient.
*  Introduction of new concepts: students first gets exposed to the terminology, theory and skills.

   At this phase students should gain some level in comfort in interacting with the new material. The new topic should no longer seem "Greek" (granted we tend to start using
   quite a couple of Greek symbols in certain topics) and the student can now read and understand basic notes and examples as well as understand and use terminology when interacting
   with a teacher.
*  Beginning acquisition of new concepts: student starts demonstrate understanding of the new material, usually by working on practice problems.

   There are two schools of thought in how this is done best. First there is the "inquiry-based learning" approach, where students take the lead in exploring the new topic, generating
   their own questions and strategies on how to proceed. The teacher will then act as a guide, providing the necessary scaffolding and assisstance to the student in this process.
   This approach seems to be a hot buzzword these days but care has to be taken in implementing it correctly. Research have often shown pure, unassisted discovery based learning
   to be ineffective. "Enhanced discovery", on the other hand, has been linked to favorable educational outcomes.

   There is also the "direct instruction" approach where a teacher provides explicit instructions and steps to guide a student in learning. There is a bit of a stigma
   for this approach sometimes as opponents to this method consider it rote learning purely based on memorization and drilling. It is often associated with boring and
   monotonous non-creative learning. While that could be the outcome if it is implemented poorly, research has shown that direct instruction can lighten the load on students'
   working memory, improve educational outcomes and even lead to more creative learning.

   As such, we think that it's important to incorporate both elements in students' learning. More important than the approach is how effectively each method is implemented.
*  Practice, review and mastery: the path from beginner to mastery is not a linear process. Often, as we get more proficient in the new concepts and techniques,
   incorrect assumptions and techniques are picked up simultaneously as well. Thus critical review is important as it allows us to identify such incorrect concepts, unlearn them
   and proceed to a higher plane of understanding.

Chart of plans
^^^^^^^^^^^^^^^^^^^^^^

+--------------+--------------------------------+-------------------------+-------------------------------+
|              | Mobile                         | Computer                | Physical                      |
+==============+================================+=========================+===============================+
| Background   | -   Math Atlas (mobile)        |                         |                               |
|              |                                |                         |                               |
|              | Quick questions                |                         |                               |
+--------------+--------------------------------+-------------------------+-------------------------------+
| Introduction |                                | (YouTube lectures)      | (School lectures)             |
+--------------+--------------------------------+-------------------------+-------------------------------+
| Practice     |                                | -   Math Atlas (online) | (Worksheets and TYS)          |
|              | -   Math Atlas (mobile)        | -   Math Bounty (PDF)   +-------------------------------+
|              | -   Math Atlas Plus (mobile)   | -   Math Bounty Plus    | -   Math Bounty (PDF)         |
|              |                                |                         |                               |
|              | Randomly generated questions   |                         | Randomly generated worksheets |
+--------------+--------------------------------+-------------------------+-------------------------------+
| Review       | -   Math Atlas (mobile)        | (YouTube solutions)     | (Classes and consultations)   |
|              |                                |                         |                               |
|              | Marking rubric                 |                         |                               |
+--------------+--------------------------------+-------------------------+-------------------------------+
| Mastery      |                                | -   Math Continental    | (Tests and exams)             |
+--------------+--------------------------------+-------------------------+-------------------------------+
| Others       | -   Math Atlas                 | (Either Math Atlas      | (Official PDF)                |
| (List MF26)  |                                | or official PDF)        |                               |
|              | Mobile optimized MF26          |                         |                               |
+--------------+--------------------------------+-------------------------+-------------------------------+

Development roadmap
^^^^^^^^^^^^^^^^^^^^^^

Math Atlas
~~~~~~~~~~~~

Synopsis: mobile app which generate random questions and marks student's attempts

Main audience for Math Atlas: students (for their own practice), teachers (for assigning homework)

Main audience for Math Atlas Plus: tutors (as a handy companion for effective direct instructions. Tutor can show how a question done as an example. Student can then proceed
to practice the same question with a few different elements).

Completed features:

*     13 randomly generated questions with interactive flow to key in answers. Students' answers marked with a marking rubric with partial credit.
*     Mobile optimized List MF26
*     Android app and web-based app.
*     Lightweight: small file size, works offline

Development plan:

*     (High priority) Bug fixes
*     (Medium priority) Saved user stats and achievements
*     (Medium-low priority) Provide more feedback to student
*     (Medium-low priority) More content: questions. Potential addition of statistics questions.
*     (Medium-low priority) IPhone app: to do if there is good adoption of the app on android.
*     (Low priority) Update questions 0101-0501 to use the Student Input/Radio classes.
*     (Low priority) Use of a local nodeJS system to generate html+javascript file from a template tex file.
*     (Low priority) Quick questions optimized for commute.

Math Bounty
~~~~~~~~~~~~~

Synopsis: web app which generate random questions and compile both question and short answers in a PDF worksheet

Main audience for Math Bounty: students (for their own practice), teachers (for creating tutorial and homework worksheets)

Main audience for Math Bounty Plus: teachers (fully customizable worksheets. We can customize the length of the worksheet based on the total marks.
We can create different worksheets for different purposes. Do we want variation of the same question for drilling? A topical worksheet covering
the entire topic for exposure? A multi-topic worksheet as test preparation? 

Development plan:

*     (High priority) Randomly generate questions in PDF worksheet form
*     (High priority) Translation of PDF form to mobile optimized form (Math Atlas Plus/Math Continental)
*     (Medium priority) New question content to fill in gaps of the initial 13 Math Atlas questions
*     (Low priority) User options to filter type of questions generated in worksheet (Math Bounty Plus) 

Math Continental
~~~~~~~~~~~~~~~~~

Synopsis: more advanced mobile app built on a different framework compared to Math Atlas

Development plan:

*     (Low priority) Use of Vue framework? Component based approach to enable better interactivity.
*     (Low priority) Work with mathlive.io to accept more advanced student inputs?
*     (Low priority) Use of native script framework?
*     (Low priority) Online integrated? Allows access to other apis. Potentially store students' attempts for analysis.
*     (Low priority) Test mode: student completes test in timed setting which are marked at the end?