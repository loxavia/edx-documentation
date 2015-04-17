.. _Documentation Translation Process:

#########################################
Documentation Translation Process
#########################################

Before you begin an edX documentation translation project, you should have a
basic understanding of restructuredText and formatting in .rst files. For more
information, see :ref:`Work with edX Documentation Source Files`.

In addition, you or another person on the translation team should understand
Github repositories and the Github pull request process. For more information
about using Github, see https://help.git.com.You or another person on the
translation team should understand Github repositories and the Github pull
request process. For more information, see https://help.git.com.

To translate edX documentation, follow these steps.

#. Use Github to clone the ``edx-documentation`` repository to a location on
   your local file system.

#. Language folders, including ``en_us``, are placed one level below 
   ``edx-documentation``. If the language you are translating into does not already
   exist, duplicate the entire ``en_us`` structure in the repository to the
   same level. Then, rename only the ``en_us`` folder with your translation
   target language, using ISO standard language-locale pairs, such as
   ``fr_ca``,``fr_fr``, ``zh_tw``, ``zh_cn``, and so on. The resulting folder
   is your working source directory.

#. Follow best practices for Github use. For information, see https://help.github.com.

	* Create a working branch for your changes. Before making new branches,
	  check that your version of “edx-documentation/master” is up to date. 
	* On your branch(es), make edits to the source files using your preferred
	  text editor. 
	* Save changes in the source files without renaming or moving the files.
	* Commit changes back to Github. 
	* Create pull requests in Github for review purposes.

4. Build draft output and make sure everything renders as it should in both
   HTML and PDF formats. 

#. Notify the edX Documentation team when you have changes ready for review
   and testing. The team might also be able to help you to generate draft
   output for review and testing.

#. Make any revisions resulting from reviews and testing, then notify the edX
   Documentation team that the pull request is ready to merge into the repository.

#. The edX Documentation team merges translation pull requests into the
   repository.

#. The edX Documentation team builds updates documentations projects for the
   next release or a planned future release.


For information about working with edX Documentation source files, see
:ref:`Work with edX Documentation Source Files`.

For documentation translation guidelines, see :ref:`Documentation Translation
Guidelines`.


