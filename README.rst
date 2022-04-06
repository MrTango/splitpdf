splitpdf
========

splitpdf can split multi page pdf files into single page files. It also allows you to provide a regular expression to find an identifier in the pdf, for example a customer id and uses it for the file name.

Installation
------------

.. code-block:: sh

    pip3 install splitpdf

or

.. code-block:: sh

    pipx install splitpdf


Usage
-----

.. code-block:: sh

    splitpdf /home/heinz/pdfinput/mylongpdffile.pdf /home/heinz/pdfoutput

Define the `SPLITPDF_IDENTIFIER_REGEX` variable to define a regular expression, which matches the identifier, for example a customer id.

On Linux you can do this in the terminal by do the following:

.. code-block:: sh

    export SPLITPDF_IDENTIFIER_REGEX="K\/\d{5}"

This will match customer id's like `K/08151`.
