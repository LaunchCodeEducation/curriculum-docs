Admonitions
===========

Admonitions call attention to content by placing it in a box with a label. RST provides several directives for creating admonitions with specific titles and styles, as well as a generic admonition with a title specified by the author.

==================  ============================
Admonition          Directive
==================  ============================
Note                ``.. note::``
Warning             ``.. warning::``
Tip                 ``.. tip::``
Question            ``.. admonition:: Question``
Example             ``.. admonition:: Example``
Examples            ``.. admonition:: Examples``
Try It!             ``.. admonition:: Try It!``
Fun Fact            ``.. admonition:: Fun Fact``
==================  ============================

Avoid using other RST admonitions, as well as over-using custom admonitions. Custom admonitions should not be used for one-off or limited-use purposes. If you feel the urge to call attention to content with a specific title, consider using a section heading.

Admonition Usage
----------------

Strive to use admonitions consistently. Admonitions are effective only when they enhance the readability of a text. If admonition usage is inconsistent, then readers will learn to ignore the titles, decreasing the effectiveness of all admonitions.

.. note:: 

   The Note is probably the most widely used admonition. It should be used to call attention to an important point. Often, Notes will also deviate from the main flow of discussion a bit. 

.. warning:: 

   Use a Warning to emphasize a subtle or surprising fact that could cause students trouble.

.. tip:: 

   Use a Tip to offer a helpful hint or piece of advice.

.. admonition:: Question

   Questions are most often used in "Check Your Understanding" sections, and block out a self-check question that the reader should consider.

.. admonition:: Example

   Examples provide concrete instances of the topic at hand.

.. admonition:: Examples

   Like an Example, but plural (duh).
   
.. admonition:: Try It!

   Try It! admonitions call the reader to learn by doing. Use Try It! with a prompt or program that the reader should engage with to better understand a concept.

   A common pattern is to follow a Try It! with a Question related to the prompt.

.. admonition:: Fun Fact

   An interesting, but supplemental, fact related to the current discussion. Fun Fact admonitions should communicate to the reader that the content is not part of the lesson's objectives, but is something that might be interesting or useful. 
