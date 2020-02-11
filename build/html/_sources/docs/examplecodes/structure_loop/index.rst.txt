.. _structure_loop_index:

Example Code: Case Structure
============================

Overview
^^^^^^^^

This example VI demonstrates case structures, including a binary case structure and a multi-state case structure.

.. figure:: case_structure_front_panel.png
  :align: center
  :scale: 60%

  `Front panel of case_structures.vi`

.. figure:: case_structure_block_diagram.png
  :align: center
  :scale: 60%

  `Block diagram of case_structures.vi`

Behavior
^^^^^^^^

#. Binary Case Structure

   The case structure should show either "This is The True Case" or "This is The False Case" string depending on the initial boolean input (push button).

#. Multi-state Case Structure

   The case structure should show corresponding string output depending on the initial string in the Enum control.

:download:`case_structures.vi <case_structures.vi>`

Example Code: For Loop
======================

Overview
^^^^^^^^

This example VI demonstrates a nested for loop indexing and outputing the elements of a predefined 2-D array.

.. figure:: for_loop_front_panel.png
  :align: center
  :scale: 60%

  `Front panel of for_loop.vi`

.. figure:: for_loop_block_diagram.png
  :align: center
  :scale: 60%

  `Block diagram of for_loop.vi`

Behavior
^^^^^^^^

The "result" indicator should show the elements of the predefined array one by one each second, while the "inner loop #" and the "outer loop #" shows the current number of iterations in the inner and outer for loop. The program should stop after iterating all the elements in the input 2-D array.


:download:`for_loop.vi <for_loop.vi>`

Example Code: While Loop
========================

Overview
^^^^^^^^

This example VI demonstrates a while loop including a meter and two LEDs (inside and outside loop) that can be controled using the knob and and the push button during execution.

.. figure:: while_loop_front_panel.png
  :align: center
  :scale: 60%

  `Front panel of while_loop.vi`

.. figure:: while_loop_block_diagram.png
  :align: center
  :scale: 60%

  `Block diagram of while_loop.vi`

Behavior
^^^^^^^^

Once excecuted, the program will keep running until the stop button is pushed. The meter indicator can be adjusted by the knob control in real time. LED2 indicator can be turned on and off by the inside loop push button. However, LED1 can only be turned on by the outside loop push button if it is pushed before execution.

:download:`while_loop.vi <while_loop.vi>`

