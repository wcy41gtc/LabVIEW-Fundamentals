.. _daqintro_index:

Data Acquisition Systems
========================

.. figure:: ./images/daq_ni.png
  :align: center
  :scale: 60%

  `A data acqusition system (Image: NI.com) <http://www.ni.com/data-acquisition/what-is/>`_

Data acqusition systems consist of three main components:

#. Sensors to measure physical systems.
#. Signal conditioning/conversion.
#. A computing device with interfacing drivers and software for data monitoring/collection.

Sensors
^^^^^^^

.. figure:: ./images/loadcell.jpg
  :align: right
  :scale: 100%

  `An S beam load cell  (Image: omega.com) <http://t0.gstatic.com/images?q=tbn%3AANd9GcSB1OSzneITOKJS24IgPwrPvN3oWgLkV0Zln0aDidu271lG6Ox5wQ61nyRI73_j9KTLfqH1g-G_&usqp=CAc>`_

Sonsors are sometimes called `transducers`, they are devices that covert physical quantities in the real world to electrical signals such voltage, current and resistance, etc. Most sensors needs electric excitaion (DC/AC power supply) and will output either analog or digital signals representing measured physical quantities.

=============== =============
       Common Sensors
-----------------------------
Sensors         Phenomenon
=============== =============
Thermocouple    Temperature
Photo Sentor    Light
Microphone      Sound
Loadcell        Force
Strain gauge    Strain
Accelerometer   Acceleration
Hygrometer      Humidity
Seismometer     Ground motion
=============== =============

Signal Conversion/Conditioning
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Signal conversion and conditioning are the essential components of a data acquisition system. The output signals from the sensors can be catagorized as **Analog** and **Digital**.

Analog Signal
^^^^^^^^^^^^^

Analog signals cover a wide range of physical phenomenon. The colors we see, the tones we hear, the temperatures that we feel, etc. There are infinite numbers of such analog signals.

In the perspective of data acquisition, analog signals are continuous and features three primary characteristics:

1. Level (Amplitude)
2. Shape
3. Frequency

.. figure:: ./images/analogsig.jpg
  :align: right
  :scale: 75%

  `Primary characteristics of an analog signal  (Image:ni.com) <https://ni.scene7.com/is/image/ni/clip_image001_20080722134950?scl=1>`_

Common analog signals include voltage, current, resistance, etc. Analog signals always inherently contain some degree of noise. Therefore, signal conditioning is usually needed for raw analog signals. Analog signals also need to be convereted to digital signals for communication and storage in computing devices.

Digital Signal
^^^^^^^^^^^^^^

Digital signals are finite, with a predefined range, meaning there is a limited values set they can be. How many values in a predefined values set depends on the total number of levels defined in the set. Due to the binary nature of modern computing devices, the number of levels is defined by  2\ :sup:`N`, where the exponent **N** is called ``bit``, the ``bit`` value is widely adopted in the industry for representing the resolution of digital signals.

Digital signals are discrete and features two primary characteristics:

1. State
2. Rate

.. figure:: ./images/digitalsig.jpg
  :align: right
  :scale: 75%

  `Primary characteristics of an digital signal  (Image:ni.com) <https://ni.scene7.com/is/image/ni/021afe6997?scl=1>`_

Driver/Software Interfaces
^^^^^^^^^^^^^^^^^^^^^^^^^^

PLace holder

Contents:

.. toctree::
   :maxdepth: 1