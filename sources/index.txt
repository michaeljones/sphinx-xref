xref Role
=========

Below are examples of the xref role using the following dictionary value for the
``xref_links`` config variable.

.. code-block:: python

   xref_links = {
                   "sphinx": ("Sphinx, the documentation generator,", "http://sphinx.pocoo.org/")
             }

**Example 1**

   ::

      This is my link to :xref:`sphinx` using the ``xref`` role.
      
   Renders as:

      This is my link to :xref:`sphinx` using the ``xref`` role.

**Example 2**

   ::

      This is :xref:`my link to Sphinx <sphinx>` using the ``xref`` role.
      
   Renders as:

      This is :xref:`my link to Sphinx <sphinx>` using the ``xref`` role.


