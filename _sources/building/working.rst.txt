Working With An Existing Module Site
====================================

To edit and publish content on an existing curriculum site, make sure
you have the necessary prerequisites and have set up Sphinx, as detailed
in `Setting Up A New Module Site <setup.html>`__.

Building the Site
-----------------

Clone the repository and, from the project directory, verify that you
can build the site.

::

   $ ./build.sh
   Running Sphinx v1.7.2
   loading pickled environment... not yet created
   building [mo]: all of 0 po files
   building [html]: all source files
   updating environment: 1 added, 0 changed, 0 removed
   reading sources... [100%] index                                                                     
   looking for now-outdated files... none found
   pickling environment... done
   checking consistency... done
   preparing documents... done
   writing output... [100%] index                                                                      
   generating indices... genindex
   writing additional pages... search
   copying static files... done
   copying extra files... done
   dumping search index in English (code: en) ... done
   dumping object inventory... done
   build succeeded.

   The HTML pages are in docs.

If the build script fails due to a permissions error, enable its
executable bit:

::

   $ chmod +x build.sh

The build script builds HTML files from the source Markdown and
reStructuredText files, using a template. It places the built files in
the ``/docs`` folder so they can be hosted via GitHub Pages.

Viewing the Site Locally
------------------------

When updating a site, you should build and proof your changes locally
before committing them. To do this, we'll use Python's ``http.server``
module.

macOS and Linux
~~~~~~~~~~~~~~~

Add the following line to your ``~/.bash_profile`` (macOS) or
``~/.bashrc`` (Linux):

::

   alias serve='python -m http.server'

Open a second terminal window and navigate to the project's ``/docs``
folder. Then run:

::

   $ serve
   Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/) ...

You can now view the site at ``localhost:8000``. You can rebuild the
site in another window while the server is still running, and changes
will be immediately reflected.

Windows
~~~~~~~

First check to make sure you have a ``~/.bash_profile`` and a
``~/.bashrc`` file, as most Windows machines do not automatically create
these files. If they do not exist create them using the following
commands:

::

   $ touch ~/.bash_profile
   $ touch ~/.bashrc

Now add the following line to your ``.bash_profile`` if it is not
already there:

::

   if [ -f ~/.bashrc ]; then
      source ~/.bashrc
   fi

Then add the following line to your ``.bashrc`` file:

::

   alias serve='python -m http.server'

Open a second terminal window and navigate to the project's ``/docs``
folder. Then run:

::

   $ serve

You can now view the site at ``localhost:8000``. You can rebuild the
site in another window while the server is still running, and changes
will be immediately reflected.

Editing Documents
-----------------

Sites build using the LaunchCode Sphinx site template may have source
code in either Markdown (abbreviated MD, with extension ``.md``) or
reStructuredText (abbreviated RST, with extension\ ``.rst``) formats.

Most LaunchCode Education sites rely primarily on RST, though in some
cases it may be suitable to use MD source files.

reStructured Text
~~~~~~~~~~~~~~~~~

Pros
^^^^

-  Table of contents generation
-  Built-in admonition (note, warning, etc) support
-  Support for cross-page references

Cons
^^^^

-  More complicated syntax than MD
-  Less well-known among developers than MD
-  Table syntax is difficult to work with

Working with RST
^^^^^^^^^^^^^^^^

reStructuredText can have a bit of a learning curve if you're accustomed
to Markdown. That said, once you get used to the basics it has definite
advantages to using MD.

Read the `Sphinx reStructuredText
Primer <http://www.sphinx-doc.org/en/stable/rest.html>`__, and bookmark
it as a reference. A modest familiarity with RST with go a long way
toward allowing you to create rich curriculum pages.

Here are a few things to note if you're new to RST:

-  RST is sensitive to whitespace in some cases. For example, when using
   a directive, the contents of the directive must be indented to align
   with the directive name (usually 3 spaces).

-  Tables in RST require alignment of column contents and
   column-separators vertically. This is a common gotcha for those new
   to RST.

-  Headings do not require a specific character (as MD does with ``#``).
   Instead, any text underlined by a repeated occurance of the same
   character will be a heading. The level of the heading is determined
   by the order of the character used in the doc. 
   
   For example: 
   
   * Level 1 Heading ===============

   * Level 2 Heading —————

   * Another Level 1 Heading ======================= 

   * Level 3 Heading ^^^^^^^^^^

-  The `RST and Sphinx
   Cheatsheet <http://openalea.gforge.inria.fr/doc/openalea/doc/_build/html/source/sphinx/rest_syntax.html>`__
   is a good resource for getting used to RST. Note that the rendered
   examples may look slightly different visually than those given due to
   differences between Sphinx templates.

When building a site with Sphinx, you are often given robust and
descriptive warnings and errors. At first, these can seem daunting ("Why
is Sphinx always yelling at me?!") but paying attention to them can help
you keep your markup code clean and avoid issues down the road.

Markdown
~~~~~~~~

When setting up Sphinx via `our
instructions <//building/setup.html#sphinx-setup>`__ we had you install
a Sphinx extension that enables support for
`CommonMark <http://commonmark.org/>`__, a widely-used Markdown
specificaion. Note that CommonMark does not include widely-used features
such as table support, which are part of MD language extensions
(e.g. GitHub Markdown).

.. _pros-1:

Pros
^^^^

-  Simple syntax
-  Is more widely known by developers than RST

.. _cons-1:

Cons
^^^^

-  Lacks several useful features supported by RST (see above)
-  CommonMark does not support tables

Working with Markdown
~~~~~~~~~~~~~~~~~~~~~

Many developers are already familiar with Markdown syntax. However, we
still encourage all contributors to skim the `CommonMark
docs <http://commonmark.org/help/>`__ to make sure you're using features
built into CommonMark, which is a smaller spec than many others.

Tables
^^^^^^

CommonMark does not directly support Markdown tables. It is possible to
support Markdown tables in Sphinx via a source-translation approach (MD
-> RST -> HTML). As of July 2018, this feature has not been implemented,
and is in the template development backlog. If you absolutely need to
use tables in your pages, we recommend using RST instead.

Site Style
~~~~~~~~~~

When creating pages, use the `Style Guide <//guide/style.html>`__. This
guide provides some basic conventions for improving the look and feel of
curriculum sites, while providing for consistency across sites.

Deploying
---------

Once you've made some changes to the site–edit, built, test,
commit–you're ready to deploy. How to do this depends on your role.

Non-Staff Contributions
~~~~~~~~~~~~~~~~~~~~~~~

For those not on the LaunchCode Education team, the recommended
deployment mechanism is to create a pull request. This allows the team
to review your changes, and to look for common formatting issues before
deploying.

.. note:: 

   Some course instructors and TAs may be granted direct commit access to course curriculum modules, based on the circumstances. If you would like direct commit access, talk to somebody on the Education team.

Staff Contributions
~~~~~~~~~~~~~~~~~~~

All Education Team staff should have push permission for the
repositories that they're working on. Pushing changes to the GitHub repo
will automatically deploy the new files.

.. warning:: 
   
   Changes to GitHub Pages sites can take several minutes to be reflected. If you push and don't see your change, wait a few minutes and do a hard refresh of the page.
