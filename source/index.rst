.. labview-fundamentals documentation master file, created by
   sphinx-quickstart on Wed Jan 29 13:29:29 2020

LabVIEW Fundamentals for Geoscientific Research
===============================================

Welcome to the LabView Fundamentals Workshop!
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Automated data acquisition systems are widely implemented in modern scientific research. A typical data acquisition system consists of sensors, signal conditioner/converter and driver/software interafeces with computing devices for data transfer and storage.

Many sensors today come with proprietary data acquisition software which can be straightforwardly deployed on a personal computer. However, challenges remain if multiple sensors of different types and from different manufacturers need to work synchronously. LabVIEW (developed and maintained by National Instruments) is a graphical programming language for developing user friendly data acquisition software unionizing signal inputs from various types of sensors. It provides endless customization possibilities to the specific data acquisition needs in terms of quantity, frequency, filtering, and timing, etc.

This documentation site is largely inspired by the amazing work done by a previous colleague J.R. Leeman, I encourage participants to checkout his awesome project `Technique for Geoscientific Experimentation (TGE) <https://tge.readthedocs.io/en/latest/>`_.

Goals
^^^^^

#. Establish an improved understanding on sensors, output signal types, and strategies on how to build adequate and cost-effective data acquisition systems
#. Jump start on LabVIEW programming, i.e., build a simple LabVIEW Virtual Instrument (VI) for analog/digital data acquisition, visualization, and recording. Touch the concepts such as producer-consumer architecture and timing control
#. Convey principles and practices on how to test, debug, and maintain the established data acquisition system

Workshop Structure
^^^^^^^^^^^^^^^^^^

This workshop covers the following topics: 1) Introduction of typical sensors, signal types, and data acquisition workflow in the laboratory; 2) Fundamentals of Labview graphical programming and some advanced topics; 3) How to test, debug, and maintain data acquisition systems

**Workshop #1**

#. Introduction to Data Acquisition

   a. Typical sensors and signals.
   b. Data acquisition workflow.
   
#. Introduction to LabVIEW graphical programming

   a. Concepts of LabVIEW VI and its components
   b. Objects, structures, and functions.
   c. Code examples.

**Workshop #2**

#. Advanced Topics

   a. Projects, sub-VIs and type defs: establish your own LabVIEW library.
   b. Producer-Consumer architecture on multi-device data acquisition.
   c. Code examples.
   
#. Test, Debug, and Maintain Data Acquisition Systems

   a. Debug VIs and hardware.
   b. Maintain VIs and good practices in laboratory.
   
.. toctree::
   :maxdepth: 1
   :caption: Contents:

   docs/daqintro/index
   docs/workflow/index
   docs/labview/index
   docs/examplecodes/index
   docs/advanced_topics/index
   docs/resources/index

Contributors:
^^^^^^^^^^^^^

.. include:: authors.rst

