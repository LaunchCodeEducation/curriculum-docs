How To Create Curriculum
========================

Introduction
------------

This guide presents some general guidelines and best practices on
creating and presenting curriculum for LaunchCode programs. It is based
on our experience in developing and running community-oriented coding
classes for non-traditional learners, and on some accepted educational
best practices.

This guide is evolving, and is not intended to be a firm set of rules to
be followed. Feel free to adapt guidelines to your specific circumstance
and to suggest improvements. If there is something you've found works
well to facilitate learning that hasn't been included here, let us know.

If you have questions about anything in this guide, or want some input
on how to best approach your curriculum development, reach out to a
member of the Education Team.

Curriculum Components
---------------------

LaunchCode course curricula are typically broken into each of the
sections below. Even if you leverage the components in different
ways–emphasizing in-class learning over prep work–it is important to
consider the role and benefit of each component in creating a course
that helps learners obtain and master new skills.

Learning Objectives
~~~~~~~~~~~~~~~~~~~

Learning objectives define the intended outcomes of a lesson. Objectives
state in specific detail the concepts students should learn, and to what
depth they should learn them. Objectives can also be used to define how
the attainment of knowledge can be verified.

You can think of learning objectives as your unit tests for your
curriculum, and your curriculum development should follow a test-driven
development pattern. Just as unit tests define the intended behavior of
an application, learning objectives define the intended outcomes of a
lesson. Just as unit tests are often used to create "self-documenting"
code, learning objectives serve as documentation for your curriculum
that can be useful to students, TAs, and LaunchCode staff.

Here are some examples of learning objectives from a hypothetical HTML
lesson:

-  Explain what HTML stands for
-  Describe the difference between a markup language and a programming
   language, and give examples of each
-  Describe HTML document structure and associated elements, and
   properly use those elements: ``<html>``, ``<head>``, ``<body>``,
   ``<title>``
-  Describe what an HTML tag is, and give common examples (e.g. ``<p>``,
   ``<div>``, ``<span>``)
-  Describe what an HTML attribute is–including how attributes relate to
   tags–and properly use attributes

Each of these examples do one or both of:

-  Define the **knowledge** that a learner should obtain. That is, what
   is the mental concept that the learner will be able to demonstrate?
   Acquisition of the given conceptual knowledge is typically verified
   by the learner's ability to explain the concept with concrete
   examples.
-  Define the **skill** that the learner should obtain. That is, what
   should the learner should be able to do? Acquisition of the given
   skill is typically verified by demonstrated use of the skill.

These two different types of objectives, while often overlapping in
practice, are important to distinguish. We might care in some cases only
that a learner can demonstrate the ability to carry out a certain task,
and not that they demonstrate a full conceptual understanding of a task.
For example:

-  Use the rules defined by a web framework's object-relational mapping
   library to configure persistent model classes.

Here, we're specifying that it is important for a learner to be able to
use the defined rules for configuring persistent model classes, without
understanding the full mechanism of how the ORM library actually carries
out the work of persisting instances of these classes. So we may not
care if a new programmer understands the full details of how data types
of class properties are mapped to data types of columns in a relational
database.

An example in the other direction–i.e. an objective that defines
knowledge without a demonstrated skill–might be:

-  Describe how a web browser parses an HTML document and turns it into
   a rendered web page.

Here, we don't intend that a learner can actually parse a document and
render a page, but that they have a conceptual understanding of this
process.

To return to the test-driven development analogy, we encourage you to
use a test-driven approach:

1. Define the learning objectives for a lesson
2. Create or source lesson material that covers the objectives
3. Create or source activities for students to practice and reinforce
   and demonstrate the objectives

Prep Work
~~~~~~~~~

Many LaunchCode courses use a **flipped classroom** approach to deliver
lesson content outside the classroom. This is beneficial for courses
where in-class time is limited, allowing time with instructors and TAs
to be focused on helping learners overcome specific difficulties and
practice new skills.

Additionally, in an environment with learners of widely-varying
backgrounds, skill levels, and learning styles, delivering primary
learning material outside of class allows for students to work through
material in their own way. Some learners may go over material multiple
times, the first time to get a broad overview, the second to gain
in-depth understanding, and a third to focus on difficult concepts not
fully grasped in a first pass. Another learner may prefer to spend more
time gaining hands-on experience with the new concepts.

The overall goal of prep work for a lesson is to expose learners to the
concepts and skills they are to gain, and to give them a chance to
identify which of those need additional clarification or reinforcement.

In Class
~~~~~~~~

Once a learner has been exposed to a concept, valuable in-class time can
be used to help them understand and practice more difficult concepts and
to solidify their understanding. In-class time should not be used to
completely rehash the material taught in prep work.

Some activities that can be useful to this end are:

-  Conceptual review and Q&A
-  Presentation of examples, focusing on potentially confusing and/or
   important areas of the lesson
-  Hands-on practice (aka "studios") using an instructor-created
   activity
-  Peer-to-peer/group practice, such as pair programming, mob
   programming, or peer-to-peer coding challenges

Once a student has been exposed to a concept, it is vital that they have
the opportunity to practice using the concept in a supported environment
before going off to use it on their own in an assignment or project.

Assignments
~~~~~~~~~~~

Assignments are critical to ensure learners fully obtain the desired
knowledge and skills. When creating assignments, refer to the learning
objectives for the associated lessons to ensure that an assignment
covers the most important (if not all) associated learning objectives.

Assignments should have **specifications** ("specs"), which outline the
objectives and tasks for the learner. A spec should include:

-  Assignment objectives
-  Starter code and/or setup instructions
-  Learner tasks
-  Submission instructions

Assignments will most often be graded via demoing with course staff. To
that end, each assignment should have a grading rubric. This should
consist of a set of specific items that the instructor or TA should
check for to verify assignment completion. Assignment grades should be
entered in Canvas.

Evaluation
~~~~~~~~~~

Another tool to evaluate and reinforce learning is evaluation via
quizzes or tests. These can be good compliments to coding assignments,
since it is possible to cover assess more conceptual objectives.

If utilizing quizzes or tests, provide students with a set of learning
objectives to study from (typically a subset of objectives from recent
lessons). We also recommend Canvas, which provides functionality for
automatic grading (for multiple choice questions), time limiting, and
automatic grade entry.

For training on how to set up quizzes in Canvas, talk to an Education
Team member.

Content Platforms
-----------------

Canvas
~~~~~~

`learn.launchcode.org <https://learn.launchcode.org>`__

Canvas is a learning management system (LMS) used to facilitate
components of class cohorts using a packaged curriculum. Canvas is the
centralized tool for:

-  **Scheduling**: slotting specific lessons and assignments into
   specific days based on the cohort schedule
-  **Attendance**: tracking student engagement
-  **Grading**: Grades entered by automatic mean (quizzes, Vocareum) or
   manual-entry (instructors and TAs entering grades)
-  **Assessments (optional)**: administering and grading exams and
   quizzes
-  **Communication**: Announcements can be sent to courses, individual
   sections/tracks, and individual students

An important point to note is that curriculum content should not hosted
in Canvas. Curriculum modules should be scheduled within Canvas, but
hosted elsewhere. This allows multiple cohorts to be run using the same,
centralized curriculum. It also enables version control and easier
access to curriculum content.

Sphinx / GitHub Pages
~~~~~~~~~~~~~~~~~~~~~

- `education.launchcode.org <https://education.launchcode.org/>`__
- `codergirl.launchcode.org <https://codergirl.launchcode.org/>`__

Most curriculum content is hosted using GitHub Pages, using the Sphinx
static site generator to generate static pages from Markdown and RST. These sites are set up and administered by LaunchCode
staff, but access can be granted to course instructors for updating and
modifying curriculum. Source code is stored in GitHub (links below).

Each site is a curriculum module which may be all or part of a given course. The links
above collect all of the curriculum modules for LaunchCode Education programs.

GitHub
~~~~~~

- `LaunchCodeEducation <https://github.com/launchcodeeducation>`__
- `LaunchCoderGirl <https://github.com/LaunchCoderGirlSTL>`__

Starter code for assignments and other activities will be hosted in
GitHub in the LaunchCoderGirl organization. The general workflow for
students should be to fork a repository into their own account, and work
on the forked copy.

It is also encouraged that any code created for lessons be made
available via GitHub and linked from the course site.

For access to course repositories, talk to an Education Team member.
