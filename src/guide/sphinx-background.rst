How Sphinx Works
================

Sphinx is a static site generator that is based on Python and RST. Our Sphinx sites incorporate several different elements that you have already installed.
These elements can be placed into three different buckets: the theme, the template, and the continuous integration (CI) tool.
Templates are used to set the layout of a website, such as the navbar.
We use a CI tool to build the curriculum sites so that if a bad build is pushed to the repository, a previous version of the site will remain live for the students. 

The Theme
---------

Themes are used to set the design standards of a website, such as fonts and colors. The theme we use is ``sphinx-bootstrap-theme``.
``sphinx-bootstrap-theme`` controls what styles are passed to the sites. The LaunchCode version is a fork so we regularly pull in updates from the upstream if we are getting too far behind.
When updating ``sphinx-bootstramp-theme``, you should be cognizant of the versions of any of the included packages, such as Bootstrap and JQuery, have changed.
If so, you need to update ``layout.html`` in ``curriculum-book-template``. You can do so by reviewing `layout.html <https://github.com/LaunchCodeEducation/sphinx-bootstrap-theme/blob/master/sphinx_bootstrap_theme/bootstrap/layout.html>`__ in ``sphinx-bootstrap-theme`` and making the appropriate changes in ``layout.html`` in ``curriculum-book-template``.
Fetching changes from the upstream constitutes most updates made to ``sphinx-bootstrap-theme``, except for changing colors.

To change the colors specifically, you have to do the following steps to ensure that ``sphinx-bootstrap-theme`` gets the changes:

#. Clone `bootswatch <https://github.com/LaunchCodeEducation/bootswatch>`__ to your computer.
#. Locate the theme you are planning on updating. ``launchcode`` contains the styles for sites hosted on education.launchcode.org.
#. Within the directory for the theme you are hoping to update, update ``variables.less`` with the necessary changes. 
#. At the project root, run ``grunt swatch``.
#. At the project root, you will find ``index.html``. Check out that file to see your changes.
#. When you are confident in your changes, commit them to ``lc_stable``.
#. Post-build of your updates to ``bootswatch``, copy the contents of the file, ``bootstrap.min.css`` in your theme directory.
#. Open ``sphinx-bootstrap-theme`` and paste the updated contents of ``bootstrap.min.css`` in the coordinating theme directory. Push the changes to the default branch.
#. To see the updates, run the :ref:`update command <update-theme>`.

The Template
------------

``curriculum-book-template`` is the template which all of our books are built on. The template includes:

#. General settings configured in ``conf.py``. 
#. General settings for Travis, our CI tool.
#. ``launchcode.css``, which is used to set the colors and styles for our code blocks. At the time of writing, we do not have a branded Pygments theme so we have to overwrite the Pygments styling at the template level.

If you make a change in one book that the other books would benefit from, make sure to apply that change to ``curriculum-book-template``.
To pull in updates to the template to the book you are working on, fetch the changes from the upstream.

The CI Tool
-----------

We use Travis for our CI tool. When you push commits to the default branch, Travis builds the site and pushes the build to ``gh-pages``. The content on ``gh-pages`` is what is deployed to the site.
If an update is made to ``sphinx-bootstrap-theme``, Travis will fetch the updates. However, if changes are made to the ``curriculum-book-template``, you have to fetch those changes when working on your local copy and push them to the default branch to see them on the live site.

