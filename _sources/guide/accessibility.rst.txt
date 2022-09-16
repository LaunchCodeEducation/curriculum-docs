Curriculum Accessibility
========================

WCAG 2.0
--------

The internationally-accepted guidelines for web accessibility are the
`WCAG 2.0 <https://www.w3.org/TR/WCAG20/>`__, which was published by the
`W3C <https://www.w3.org/>`__. At this time, the U.S. Federal Government
has not issued separate guidelines for web accessibility.

.. note::

   The W3C released WCAG 2.1 on June 5, 2018. The addition of several success criteria may cause this page to be updated in the near future.

Those guidelines lay out success criteria for various regulations that
make websites more accessible to all readers. The guidelines are based
on four principles of accessibility:

1. Perceivable
2. Operable
3. Understandable
4. Robust

In testing curriculum pages, we offer a checklist that allows you to
navigate through your own pages and quickly assess where you stand in
terms of accessibility, as well as a list of tools that you will find
helpful in testing your pages.

Testing Curriculum Pages
------------------------

Extensions and Assistive Software for Testing
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Extensions
^^^^^^^^^^

1. `aXe <https://chrome.google.com/webstore/detail/axe/lhdoppojpmngadmnindnejefpokejbdd?hl=en-US>`__:
   published by Deque Systems, aXe runs in the Developer Tools.
   Developers can quickly analyze a page to find issues and the tool is
   built to adhere to WCAG 2.0.
2. `ChromeLens <https://chrome.google.com/webstore/detail/chromelens/idikgljglpfilbhaboonnpnnincjhjkd>`__:
   ChromeLens will also run in the Developer Tools and offers insight
   into how the page will appear to people with different vision
   impairments. The extension includes lenses that reflect how the page
   appears to people with the following:

   -  Full blindness
   -  Serious partial blindness
   -  Medium partial blindness
   -  Mild partial blindness
   -  Protanomaly
   -  Protanopia
   -  Deuteranomaly
   -  Deuteranopia
   -  Tritanomaly
   -  Tritanopia
   -  Achromatomaly
   -  Achromatopsia

Assistive Software
^^^^^^^^^^^^^^^^^^

1. Screen Reader: a screen reader will use the HTML tags to guide the
   user through the content on the page while reading the page to the
   user. Many operating systems, such as Windows and Mac, offer default
   screen readers that can be turned on in the Accessibility settings of
   System Preferences.
2. Screen Magnifier: screen magnifiers will magnify the screen to a
   level that the user selects. Both Windows and Mac offer screen
   magnifiers that can be turned on in the Accessibility settings of
   System Preferences.
3. Keyboard-enabled Browsing: many users may opt to navigate pages with
   their keyboards as opposed to a trackpad or mouse. To test whether or
   not the users can easily navigate the page, developers can turn on
   keyboard-enabled browsing in the Accessibility settings of System
   Preferences.

Run through WCAG Checklist
~~~~~~~~~~~~~~~~~~~~~~~~~~

The WCAG are incredibly long and ever-changing. A good way to test your
site's accessibility is by looking at the site through different lenses.
Steven Lambert broke down the Lenses of Accessibility in his article,
`Designing for Accessibility and
Inclusion <https://www.smashingmagazine.com/2018/04/designing-accessibility-inclusion/>`__.

1.  The Lens of Animation and Effect

    1. Are there animations or effects on this page?

       -  No: move on to the next lens.
       -  Yes: move on to the second question.

    2. Do these animations or effects serve an educational purpose?

       -  No: remove the animations or effects.
       -  Yes: if the animation or effect could cause discomfort or a
          seizure, remove them. If not, find the best way to annotate
          that animation or effect.

2.  The Lens of Audio and Video

    1. Are there elements on this page that include audio or video?

       -  No: move on to the next lens.
       -  Yes: move on to the second question.

    2. Do these elements serve an educational purpose?

       -  No: remove the elements.
       -  Yes: do these elements have the proper annotations and
          captioning?

          -  Yes: move on to the next lens.
          -  No: add the proper annotations as outlined above.

3.  The Lens of Color

    1. Is color being used to convey meaning at any point in this
       document?

       -  Yes: color should not be used to convey meaning. Reword the
          text if necessary so that color is not needed.
       -  No: move on to the next question.

    2. Are the colors in the document in proper contrast to each other?

       -  Yes: move on to the next question.
       -  No: review above for compatible color combinations

    3. Review the site with ChromeLens to check the site for various
       vision disorders.

4.  The Lens of Control

    1. Are the controls properly formatted?

       -  No: the controls are too close together, too small or within
          another control.
       -  Yes: Move on to the second question.

    2. Does each control have a visible text label?

       -  No: add a visible text label to each control.
       -  Yes: move on to the next lens.

5.  The Lens of Font

    1. Can users change the fonts and/or font sizes to what they need in
       order for them to read the website?

       -  Yes: move on to the next lens.
       -  No: accessible websites need to be adaptable.

6.  The Lens of Images and Icons

    1. Does the image serve an educational purpose?

       -  Yes: move on to the next question.
       -  No: remove the image.

    2. Does the image contain any information that would be lost if it
       was not viewable?

       -  Yes: add succinct descriptions to each image.
       -  No: Does the image need to be in the site? If so, add
          appropriate alternate text.

7.  The Lens of Keyboard

    1. Is the site ordered in a way that makes sense for keyboard users?

       -  No: Turn on keyboard navigation in your computer's System
          Preferences and check out the site to see if the page can be
          ordered better.
       -  Yes: Move on to the next lens.

8.  The Lens of Layout

    1. Does the layout of the site have a meaningful and logical
       sequence?

       -  Yes: move on to the next question.
       -  No: Reorder the site to make it work better.

    2. What happens to the layout of the screen when it is zoomed in?

       -  If it stays readable and logical, proceed forward.
       -  If not, improve the layout.

    3. Is content that is related in close proximity to one another?

       -  If not, reorder the content so that it is in close proximity
          to related content.
       -  If so, move on to the next lens.

9.  The Lens of Material Honesty

    1. Are there elements that behave or look like another element?

       -  Yes: do they need to be so? Are they making the design
          dishonest?
       -  No: move on to the next lens.

10. The Lens of Readability

    1. Is the language simple and free of too much jargon?

       -  No: edit the language to make it more readable to people at a
          variety of skill levels.
       -  Yes: Move on to the next question.

    2. Are all of the headings, links, controls and labels clear?

       -  No: edit the labels for clarity.
       -  Yes: Move on to the next lens.

11. The Lens of Structure

    1. Is the HTML structured in such a way that a screen reader can
       navigate the page?

       -  No: Restructure the HTML so that a user with a screen reader
          can easily navigate the page.
       -  Yes: Move on to the next lens.

12. The Lens of Time

    1. Is there a time limit to the page?

       -  Yes: remove the time limit.
       -  No: You have checked the whole page!

One final important step is to have another person check your page!

Colors
------

Color contrast plays a big role in determining how readable our
materials are for people with low vision. When using a evaluation tool
like aXe, color contrast errors may come up. If you see one, please note
the element that is effected so that the styling can be changed.
Contrast ratios are used as the ratio can help determine how readable
our materials are for students with low vision and color deficiencies.
The contrast can be calculated using different tools online such as
`Contrast-Ratio <https://contrast-ratio.com>`__. The acceptable ratios
will vary based on the size of the font with the ratio increasing as the
font size decreases. The acceptable ratios are:

1. 3 : 1 is the minimum acceptable level for people with standard vision
   or 20/20 vision (Level A).
2. 4.5 : 1 is the ratio required for level AA, as it compensates for
   individuals with less contrast sensitivity due to loss of vision.
   This corresponds to 20/40 vision.
3. 7 : 1 is the ratio required for level AAA. This corresponds to 20/80
   vision.


.. note::

   Someone who is legally blind has 20/200 central vision acuity.

Colors and Comparisons
~~~~~~~~~~~~~~~~~~~~~~

LaunchCode Education uses all of LaunchCode's colors. Below is a table
of compliant color combinations.

========== ========= =================== =========== ====================
Color One  Color Two Level of Compliance Color Ratio Comparison
========== ========= =================== =========== ====================
Dark Blue  White     Level AAA           9.14 : 1    `Comparison Swatches <https://contrast-ratio.com/#%23354a5f-on-white/>`__
Dark Blue  Grey      Level AA            5.58 : 1    `Comparison Swatches <https://contrast-ratio.com/#%23354a5f-on-%23cacacb/>`__
Dark Blue  Orange    Acceptable          3.31 : 1    `Comparison Swatches <https://contrast-ratio.com/#%23354a5f-on-%23f47753/>`__
Light Blue White     Acceptable          3.19 : 1    `Comparison Swatches <https://contrast-ratio.com/#%235c94ce-on-white/>`__
========== ========= =================== =========== ====================

When working with the CoderGirl sites, LaunchCode Education uses the
specific CoderGirl colors. Below is a table of compliant color
combinations.

========== ========= =================== =========== ====================
Color One  Color Two Level of Compliance Color Ratio Comparison
========== ========= =================== =========== ====================
Dark Blue  Green     Acceptable          4.1 : 1     `Comparison Swatches <https://contrast-ratio.com/#%2361c08d-on-%23354a5f/>`__
Dark Blue  Grey      Level AA            5.58 : 1    `Comparison Swatches <https://contrast-ratio.com/#%23354a5f-on-%23cacacb/>`__
Dark Blue  Orange    Level AA            4.99 : 1    `Comparison Swatches <https://contrast-ratio.com/#%23faaf79-on-%23354a5f/>`__
Dark Blue  White     Level AAA           9.14 : 1    `Comparison Swatches <https://contrast-ratio.com/#%23354a5f-on-white/>`__
Light Blue White     Acceptable          3.19 : 1    `Comparison Swatches <https://contrast-ratio.com/#%235c94ce-on-white/>`__
========== ========= =================== =========== ====================

HTML
----

As developers striving for accessible curriculum and using static site
generators, it is vital to keep an eye out on the HTML that Sphinx
produces. Many assistive technologies such as screen readers use HTML as
a way to guide through the page.

Headings
~~~~~~~~

Many screen reader users will navigate through the page first by
headings. This is why it is important to make sure that headings don't
skip levels.

What not to do: 

#. h1
#. h3
#. h2

What to do: 

#. h1
#. h2
#. h3

.. note:: With RST, it's impossible to use headings improperly in this way. However, you should be aware of proper nesting of headings when using other languages such as HTML and Markdown.

Lists
~~~~~

Providing content in a logical and ordered manner is a mandate of
accessibility guidelines. As a result, when using a list, ordered lists
should be used over unordered lists. Using an ordered list will help
users with assistive technologies navigate the page.

ARIA
~~~~

ARIA tags can be used to clarify specific aspects of a user interface.
WAI-ARIA 1.0 are the accepted guidelines regarding the use of ARIA. One
important thing to keep in mind before implementing ARIA is that no ARIA
is better than bad ARIA.

Images
------

Images are non-text content and cannot be read by a screen reader or
other assistive technology. When using non-text content, the developer
can do a number of things to make sure that the alternate text or
``alt`` used is descriptive for the user.

Alternate text
~~~~~~~~~~~~~~

In curriculum development, a lot of images used are screenshots
illustrating expected outcomes. Because of that, a short description
using ``alt`` should be supplemented with a longer description in the
text.

Videos
------

Videos are another form of non-text content. Because of the combination
of audio and video, developers should double check that they have
provided as many accessibility aids as possible.

Since many users are already accustomed to YouTube's platform, one quick
thing a developer can do to ease the user's experience can be providing
a link to the video on YouTube in addition to embedding it within the
site.

Audio
~~~~~

With time-based non-text content, audio accommodations go beyond closed
captioning.
