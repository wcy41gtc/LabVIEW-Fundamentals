.. labview-fundamentals documentation master file, created by
   sphinx-quickstart on Wed Jan 29 13:29:29 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

LabVIEW Fundamentals Workshop
=============================

Welcome to the documentations for the LabView Fundamentals Workshop!
====================================================================

Automated data acquisition systems are widely implemented in modern scientific research. A typical data acquisition system consists of sensors, data acquisition devices, and monitoring or recording devices with compatible software. Most sensors today come with proprietary data acquisition software which can be straightforwardly deployed on a personal computer. However, challenges remain if multiple sensors of different types and from different manufacturers need to work synchronously. LabVIEW (developed and maintained by National Instruments) is a popular platform for developing user friendly data acquisition software unionizing signal inputs from various types of sensors. The programming language provides endless customization possibilities to the specific data acquisition needs in terms of quantity, frequency, filtering, and timing, etc. This workshop covers the following topics: 1) Introduction of typical sensors, data types, and data acquisition hardware used in the laboratory; 2) Fundamentals of Labview graphical programming and producer-consumer architecture; 3) How to test, debug, and maintain data acquisition systems

Goals
=====

1.	Establish an improved understanding on sensors, output signal types, and strategies on how to build adequate and cost-effective data acquisition systems
2.	Jump start on LabVIEW programming, i.e., build a simple LabVIEW Virtual Instrument (VI) for analog/digital data acquisition, visualization, and recording. Touch the concepts such as producer-consumer architecture and timing control.
3.	Convey principles and practices on how to test, debug, and maintain the established data acquisition system.

Structure
=========

Introduction to Data Acquisition
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
1.	Overview of data acquisition in scientific research
2.	Transducers
3.	Analog vs. Digital Signals
4.	Common Data Acquisition Hardware, drivers, and Software
5.	Data Acquisition Workflow

Build Customized Data Acquisition Software with LabVIEW
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
1.	Introduction to LabVIEW graphical programming
2.	Analog, digital, and visual image data acquisition modules and utilities.
	2.1.	Write a simple virtual instrument (VI) program with a GUI using LabVIEW.
	2.2.	Visualization and real-time monitoring/processing of data.
	2.3.	Format and save the acquired data.
3.	Advanced Topics
	3.1.	Projects, sub-VIs and type defs: establish your own LabVIEW library.
	3.2.	Producer-Consumer architecture.
	3.3.	Data synchronization.
	3.4.	Timing control on multi-device data acquisition.

Test, Debug, and Maintain Data Acquisition Systems
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
1.	Common issues and misconducts in laboratory regarding electronics.
2.	Proper precautions on protecting data acquisition systems.
3.	Noise and how to deal with them.
4.	Debug VIs and hardware.
5.	Maintain VIs and good practices in laboratory.


Links
^^^^^

.. toctree::
   :maxdepth: 2
   :caption: Contents:


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
