.. _Documentation Translation Guidelines:

###############################################
Guidelines for Translators
###############################################

This section provides basic guidelines for translators of edx documentation.
The complete edX documentation translation process is described in
:ref:`Documentation Translation Process`.

.. note:: Before you begin an edX translation project, you should have a basic
   understanding of restructuredText and formatting in .rst files. For more
   information, see :ref:`Work with edX Documentation Source Files`.

   In addition, you or another person on the translation team should
   understand Github repositories and the Github pull request process. For
   more information about using Github, see https://help.git.com.

When you translate edX documentation source .rst files, follow these
general guidelines.

.. warning:: Do not rename or move folders or files (including .rst, .png).
   The location and names of files in your language folder structure should
   exactly match that of the en_us folder structure.

*************************
What To Translate
*************************

In addition to obvious text, do translate the following items.

* Note and Warning text. Translate text following the tags ``.. note::`` or
  ``.. warning::`` Be careful to wrap and indent lines correctly.

* Link text in inline links. Translate text following the tag ``:ref:``
  Be careful not to modify the referenced link anchor.
* Alt text in images. Translate text following the tag ``:alt:``.

*****************************
What Not to Translate
*****************************

Do not translate or alter any of these elements.

* The filenames and locations of any .rst files in the repository.
* Any part of the .rst tags listed in :ref:`Work with edX Documentation Source
  Files` and :ref:`SampleRSTFile<Anchor For SampleRSTFile>`. 
* File paths in image references. 
* The text of anchors in .rst files. 
* Code examples that are tagged with ``..code-block::``.  
* Variables or database field names that are tagged with
  monospace code font (double grave accent characters).

For information about working with edX Documentation source files, see
:ref:`Work with edX Documentation Source Files`.

For information about the documentation translation process, see
:ref:`Documentation Translation Process`.
