.. labview-fundamentals documentation master file, created by
   sphinx-quickstart on Wed Jan 29 13:29:29 2020

LabVIEW Fundamentals for Geoscientifc Research
==============================================

Welcome to the documentations for the LabView Fundamentals!
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Automated data acquisition systems are widely implemented in modern scientific research. A typical data acquisition system consists of sensors, data acquisition devices, and monitoring or recording devices with compatible software. Most sensors today come with proprietary data acquisition software which can be straightforwardly deployed on a personal computer. However, challenges remain if multiple sensors of different types and from different manufacturers need to work synchronously. LabVIEW (developed and maintained by National Instruments) is a popular platform for developing user friendly data acquisition software unionizing signal inputs from various types of sensors. The programming language provides endless customization possibilities to the specific data acquisition needs in terms of quantity, frequency, filtering, and timing, etc. This workshop covers the following topics: 1) Introduction of typical sensors, data types, and data acquisition hardware used in the laboratory; 2) Fundamentals of Labview graphical programming and producer-consumer architecture; 3) How to test, debug, and maintain data acquisition systems

This short workshop will guide you through the fundamentals of data acquisition systems and basic LabVIEW programming.

This documentation is largely inspired by the amazing work done by my previous colleague J.R. Leeman, I encourage participants to checkout and contribute to his awesome project `Technique for Geoscientific Experimentation (TGE) <https://tge.readthedocs.io/en/latest/>`_.


Goals
^^^^^

#. Establish an improved understanding on sensors, output signal types, and strategies on how to build adequate and cost-effective data acquisition systems
#. Jump start on LabVIEW programming, i.e., build a simple LabVIEW Virtual Instrument (VI) for analog/digital data acquisition, visualization, and recording. Touch the concepts such as producer-consumer architecture and timing control
#. Convey principles and practices on how to test, debug, and maintain the established data acquisition system

Workshop Structure
^^^^^^^^^^^^^^^^^^

#. Introduction to Data Acquisition

   a. Data acquisition in geoscientific research
   b. Typical Transducers and Signal Types
   c. Data Acquisition Workflow
   
#. Build Customized Data Acquisition Software with LabVIEW

   a. Introduction to LabVIEW graphical programming
   b. Analog, digital, and visual image data acquisition modules and utilities
   c. Virtual instrument (VI) with a GUI using LabVIEW
   d. Format and save the acquired data
   
#. Advanced Topics

   a. Projects, sub-VIs and type defs: establish your own LabVIEW library
   b. Producer-Consumer architecture
   c. Data synchronization
   d. Timing control on multi-device data acquisition
   
#. Test, Debug, and Maintain Data Acquisition Systems

   a. Common issues and misconducts in laboratory regarding electronics
   b. Noise and how to deal with them
   c. Debug VIs and hardware
   d. Maintain VIs and good practices in laboratory
   
.. toctree::
   :maxdepth: 2
   :caption: Contents:

   docs/hardware/index
   docs/transducers/index
   docs/signals/index
   docs/workflow/index
   docs/labview/index
   docs/examplecodes/index
   docs/advanced_topics/index
   docs/resources/index

Contributors:
^^^^^^^^^^^^^

.. include:: authors.rst


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
