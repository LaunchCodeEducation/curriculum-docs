Contributing a Pull Request
===========================

Fork and Clone the Textbook Repository
--------------------------------------

Your first step in making a contribution to our open-source textbooks is to grab a copy
of the code for the book site you want to change. The book site name will tell you 
where to go to find the repository.

For example, if you want to make a change to the book at 
https://education.launchcode.org/intro-to-professional-web-dev,
you'll find this repository at https://github.com/LaunchCodeEducation/intro-to-professional-web-dev.

From that GitHub page, use the 'Fork' button to fork a copy to your GitHub profile.

.. admonition:: Note
    
    If you are a member of the LaunchCodeEducation organization on GitHub,
    you do not need to use a forked copy of the repository and can instead 
    simply clone the repository you want to edit.

Clone the forked repository onto your computer:

::

   $ git clone git@github.com:LaunchCodeEducation/intro-to-professional-web-dev.git

Alternatively, if you don't have an SSH key configured for your GitHub
account, use HTTPS:

::

   $ git clone https://github.com/LaunchCodeEducation/intro-to-professional-web-dev.git


With a copy of the code for the book, you'll next have to build the program on your computer.
First, you have to setup your computer with some dependencies to get the text built.

Prerequisites
-------------

Python
~~~~~~

Working with our Sphinx setup requires Python 3.5+.

Check your Python version:

::

   $ python -V
   Python 3.6.1 :: Continuum Analytics, Inc.

On some systems, Python 3 will be installed as ``python3``:

::

   $ python3 -V
   Python 3.6.5

.. note::

   If you are using ``python3``, you'll need to use ``pip3`` wherever ``pip`` is used in the sections below.

If you don't have a sufficient Python install, we recommend installing
`Miniconda <https://conda.io/miniconda.html>`__.

Sphinx Setup
------------

Install `Sphinx <http://www.sphinx-doc.org/en/master/>`__:

::

   $ pip install sphinx==3.3.1

Install
`Recommonmark <https://recommonmark.readthedocs.io/en/latest/>`__ to
allow for writing of Markdown files in Sphinx:

::

   $ pip install recommonmark

Install the LaunchCode fork of the ``sphinx-bootstrap-theme`` Sphinx
theme.

::

   $ pip install git+https://github.com/LaunchCodeEducation/sphinx-bootstrap-theme.git@master

Install pypandoc because if you don't, you will see an error after
running build

::

   $ pip install pypandoc


Building the site
~~~~~~~~~~~~~~~~~

Now build the site using the *build* script in the project's root directory.
To do this, open a terminal window and navigate to the project's root directory.
Use the command below to build. If all is setup correctly, you will start to see the build
logs look something like those below.

::

   $ ./build.sh
   Running Sphinx v3.3.1
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

.. note:: 

   At this point, if you wish to view the site locally, the build command will have created a new 
   directory in the project called *docs/*. Open this directory and find *index.html*.
   Right click on the file name for *index.html* and select *Copy Path*. Drop this into 
   your browser of choice (not Internet Explorer, please). You should see the built site running.

Adding, Committing, and Pushing Your Suggested Changes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Be sure to make your changes on a feature branch so that you can create a PR off master
for the LaunchCode team to review.

::

   $ git add .
   $ git commit -m "Initial build"
   $ git push origin master

Once pushed, `open a PR on GitHub <https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request>`__ and we'll be in touch to review your work and
get your contributions merged in and deployed.

