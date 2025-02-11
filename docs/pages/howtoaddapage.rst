How to add a new page
=====================

The first step is to consider whether your file should be an addition to 
an existing SOP, or should be the start of a new SOP tree. Let's explore the difference.

If you are adding to an existing file:

- Open that file, make changes, commit those changes, and push it to the main branch.

If you need to create a new SOP file:

1. Head over to the "QMG-wiki/docs/pages" directory and make a "mynewpage.rst" file.

2. Write your new sop using the reStucturedText_ syntax

.. _reStucturedText: https://github.com/ralsina/rst-cheatsheet/blob/master/rst-cheatsheet.rst

3. Make reference to this file in this file in the "/docs/index.rst" toctree (table of contents).
4. Stage, Commit and push all your changes to the main branch.

Always! Check your changes have rendered the way you expect on the QMG-wiki readthedocs_.

.. _readthedocs: http://qmg-wiki.rtfd.io/

Note: Images should be stored in "/docs/_static/". Either directly or for multiple pictures in a folder.

To reference these pictures in your SOP use: 

.. code-block:: rst
    
    Below is an image of a pixel cat.
    
    |pixelcat|

    .. |pixelcat| image:: ../_static/pixelcat.png
        :width: 45% 


Below is an image of a pixel cat.

|pixelcat|

.. |pixelcat| image:: ../_static/pixelcat.png
    :width: 45% 
