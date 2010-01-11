sphinx xref role
================

This is a simple restructured text role which aims to make it easier to link
repeatedly to external documentation.

The role allows you to provide a dictionary of keywords which map to urls so
that instead of repeating the urls throughout your documentation you can use
the keywords instead. 

In addition to being more readable when working with the source text, it allows
a list of urls and keywords to be maintained separately and, if desired,
programmatically making them easier to update.

Also multiple sets of documentation using the same keyword-url dictionary can
be kept up to date by maintaing a single central module with the dictionary as
opposed to links scattered through several texts.

Example
-------

Using the following dictionary setup in the Sphinx config file:

    xref_links = {
        "sphinx": ("Sphinx, the documentation generator,", "http://sphinx.pocoo.org/")
        }

The restructured text:

    This is my link to :xref:`sphinx` using the ``xref`` role.

Will render as:

 This is my link to [Sphinx, the documentation generator,](http://sphinx.pocoo.org/) using the `xref` role.


The advantages become more apparent with scale.

Credits
-------

Thank you to Georg Brandl for [Sphinx](http://sphinx.pocoo.org/) and David
Goodger for [Docutils](http://docutils.sourceforge.net/).



