.. _Anchor For SampleRSTFile:

#################
Sample .rst File
#################


.. _Anchor for Heading One:

################################
Heading One has hash characters
################################

Headings are text sandwiched between rows of specific characters. The row of
hash, asterisk, or equals characters must be as long as, or longer than, the
text of the heading. If the translated heading string is longer than the
original English source, make sure you extend both lines above and below the
heading string.

This is regular text in paragraph form. There are no indents. As a best
practice, break lines at about 80 characters, so that each line has its own
line number for commenting in reviews. This is regular text in paragraph form.
There are no indents. As a best practice, break lines at about 80 characters,
so that each line has its own line number for commenting in reviews.

.. comments can be added in a file by starting a line with 2 periods and a space. 

In English source files, look for comments addressed to translators from writers.


.. note:: This is note text. If note text runs over a line, make sure the
   lines wrap and are indented to the same level as the note tag. If
   formatting is incorrect, the entire note might not render in the HTML
   output.

   Notes can have more than one paragraph. Successive paragraphs must indent
   to the same level as the rest of the note.


.. warning:: Warnings are formatted in the same way as notes. In the same way,
   lines must be broken and indented under the warning tag.


.. _Anchor for Heading Two:

************************************
Heading Two has asterisk characters
************************************

A cross-reference link looks like this: See :ref:`Anchor for Heading One`. In
HTML and PDF output, the actual title text of Heading One is substituted for
the reference tagging, and provides a link to the target location. Actual
anchor text is never visible in output.

To create an inline link whose text is different from the actual title text of
the target heading, you :ref:`make a link like this<Anchor for Heading One>`,
where you place the anchor text within angle brackets immediately following
the link text. In HTML and PDF output, the text "make a link like this" would
appear as a link and provide a link to the topic with the anchor "Anchor for
Heading One".


To create a numbered list, start lines with a pound sign followed by a period.

.. note:: if the numbered list is interrupted by extra formatting, it might be
   necessary to explicitly enter a number in place of the pound sign so that
   the numbered list does not restart at 1. For example, see Step 3 in the
   following procedure example.


#. Switch to the **HTML** tab. 

#. Replace the following placeholders with your own content.

   * Replace the value of the <a> element's href attribute with the path to
     your image. Do not change the value of the class attribute. For example:

     **<a href="/static/Image1.jpg" class="modal-content">**

   * Replace the value of the <img> element's src attribute with the path to
     your image. For example:
     
     **<img alt="Full screen image" src="/static/Image1.jpg"/>**

   * Ensure that the value of the href and src attributes are the same, and
     that you do not change the class attribute. Your sample code should look
     like the following:

   .. code-block:: xml

     <h2>Sample Image Modal</h2>
     <a href="/static/Image1.jpg" class="modal-content">
     <img alt="Full screen image" src="/static/Image1.jpg"/>
     </a>

   .. note:: You can use this same HTML code in any HTML component, not just
      those components you created as full screen images.

3. Click **Save** to save the HTML component.


=====================================
Heading Three has equals characters
=====================================

Image references look like this. 

.. image:: ../../../shared/building_and_running_chapters/Images/about_page.png
   :alt: An image of the course summary page.

Some image links might have additional specifications such as height, width,
or scale.

Alternative text for screen readers is required for each image. Provide text
that is useful to someone who might not be able to see the image.

When you translate existing content, make sure you do not change the filepath
portion of the image reference. You should only translate the alternative
text.


************************************
Tables
************************************

Tables look like this. Each row is indicated with an asterisk. Each column in
a row is indicated with a hyphen. The following table has three columns. There
is a single space between the asterisk and the hyphen. Note that the asterisks
must all align, and the hyphens must all align. Empty cells must be accounted
for, so that each column in a row is always marked, even if there is no
content in a table cell.


.. list-table::
   :widths: 25 25 50

   * - .. image:: ../../../shared/building_and_running_chapters/Images/AnnotationExample.png
          :width: 100
          :alt: Example annotation problem
     - 
     - Annotation problems ask students to respond to questions about a
       specific block of text. The question appears above the text when the
       student hovers the mouse over the highlighted text so that students can
       think about the question as they read.
   * - .. image:: ../../../shared/building_and_running_chapters/Images/PollExample.png
          :width: 100
          :alt: Example poll
     - 
     -  You can create a conditional module to control versions of content that
        groups of students see. For example, students who answer "Yes" to a
        poll question then see a different block of text from the students who
        answer "No" to that question.
   * - .. image:: ../../../shared/building_and_running_chapters/Images/JavaScriptInputExample.png
          :width: 100
          :alt: Example JavaScript problem
     - 
     - Custom JavaScript display and grading problems (also called *custom
       JavaScript problems* or *JS Input problems*) allow you to create a
       custom problem or tool that uses JavaScript and then add the problem or
       tool directly into Studio.
  

************************************
Code Examples
************************************

===========
Inline code
===========

In inline text, any text can be formatting as code (monospace font) by
enclosing the selection within a pair of double "grave accent" characters. For
example, ``these words`` are formatted in a monospace font when the
documentation is output as PDF or HTML.

===========
Code blocks
===========

For larger blocks of code that are provided as examples, use the code-block tag. Here is a code block.
The type of code is indicated after the 2 colons in the tag.

        .. code-block:: xml

          <problem>
              <annotationresponse>
                  <annotationinput>
                    <text>PLACEHOLDER: Text of annotation</text>
                      <comment>PLACEHOLDER: Text of question</comment>
                      <comment_prompt>PLACEHOLDER: Type your response below:</comment_prompt>
                      <tag_prompt>PLACEHOLDER: In your response to this question, which tag below 
                      do you choose?</tag_prompt>
                    <options>
                      <option choice="incorrect">PLACEHOLDER: Incorrect answer (to make this 
                      option a correct or partially correct answer, change choice="incorrect" 
                      to choice="correct" or choice="partially-correct")</option>
                      <option choice="correct">PLACEHOLDER: Correct answer (to make this option 
                      an incorrect or partially correct answer, change choice="correct" to 
                      choice="incorrect" or choice="partially-correct")</option>
                      <option choice="partially-correct">PLACEHOLDER: Partially correct answer 
                      (to make this option a correct or partially correct answer, 
                      change choice="partially-correct" to choice="correct" or choice="incorrect")
                      </option>
                    </options>
                  </annotationinput>
              </annotationresponse>
              <solution>
                <p>PLACEHOLDER: Detailed explanation of solution</p>
              </solution>
            </problem>




