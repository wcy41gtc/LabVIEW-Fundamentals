.. _workflow_index:

Data Acquisition Workflow
=========================

A typical data acqusition workflow contains the following steps:

#. **Physical Syetem**: indentify the physical system/phynomenon.
#. **Sensors**: determine the sensor group that is appropriate for measuring the physical system.
#. **Signal Conditioning**: Condition the raw analog signal to safe and measurable range, filter noise if necessary.
#. **ADC**: Choose an appropriate `analog to digital converter` for converting the conditioned analog signal to digital signal.
#. **Computer**: Monitor and record the signal.

.. figure:: ./images/daqworkflow.png
  :align: center
  :scale: 70%

  `A Typical DAQ Workflow (Ref: J.R. Leeman TGE) <https://tge.readthedocs.io/en/latest/content/lectures/lecture_7.html>`_


Example: Axial Strain of Rock Cylinder
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In this example, we want to measure the axial strain (:math:`\epsilon`) of a cylindrical rock specimen during uniaxial compression test.

.. math::
   \epsilon=\frac{\Delta L}{L}


where :math:`\Delta L` is the change of axial length due to the compression; :math:`L` is the initial length of the specimen.

For more on mechanics and deformation please refer to the `wiki page about deformation <https://en.wikipedia.org/wiki/Deformation_(mechanics)>`_

Physical System
^^^^^^^^^^^^^^^

In a uniaxial compression test, a cylindrical rock specimen is placed vertically inside a loading frame. The load is applied on the axial direction of the rock specimen. An example of the physical system is shown below.

.. figure:: ./images/ucs.png
  :align: center
  :scale: 60%

  `The Physical System of UCS Test (Image control-group) <https://m.controls-group.com/eng/products/rock-mechanics-testing-equipment-testing-equipment-testing-equipment/strain-gauges-for-uniaxial-and-triaxial-tests>`_


Sensor: Strain Gauge
^^^^^^^^^^^^^^^^^^^^

For a small strain system scenario, a linear strain gauge is usually implemented to measure the axial strain. A strain gauge consists of an insulating flexible backing which supports a metallic foil pattern . A strain gauge is attached to the object by a suitable adhesive. As the object is deformed, the attached strain gauge is deformed as well, causing its electrical resistance to change.
(`learn more about strain gauge on Wikipedia <https://en.wikipedia.org/wiki/Strain_gauge>`_)

.. figure:: ./images/straingauge.png
  :align: center
  :scale: 60%

  `The Working Concept of a Linear Strain Gauge (Image Wikipedia) <https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/StrainGaugeVisualization.svg/400px-StrainGaugeVisualization.svg.png>`_

In practice, a `Wheatstone Bridge <https://en.wikipedia.org/wiki/Wheatstone_bridge>`_ is implemented for measuring the voltage output caused by the resistance change of the strain gauge. In this specific case, the configuration is called **quarter bridge**. A Wheatstone bridge circuit is capable of precisely measuring an unknown electrical resistance change by balancing its two legs.

.. figure:: ./images/quarterbridge.png
  :align: center
  :scale: 80%

  `The circuit diagram for a quarter Wheatstone bridge (Cimbala, 2013) <https://www.me.psu.edu/cimbala/me345/Lectures/Strain_gages.pdf>`_

The strain can be approximated by the following equation for quarter bridge configuration,

.. math::
   \epsilon \approx 4\frac{V_0}{V_S}\frac{1}{G}

where :math:`V_0` is the measured volatge; :math:`V_S` is the excitation voltage (supply voltage); :math:`G` is the gauge factor determined by the strain gauge manufacturer.

Signal Conditioning
^^^^^^^^^^^^^^^^^^^

Raw analog signals contain some degrees of interference. For example, an AC line nearby may introduce high frequency interference, the periodic temperature change over time can introduce low frequency interference. Signal filters are common signal conditioning tools to block or extract signal components of a certain frequency range.

.. figure:: ./images/hpf-lpf.png
  :align: center
  :scale: 50%

  `Passive Low Pass Filter (Image electronics-tutorials) <https://www.electronics-tutorials.ws/filter/filter_2.html>`_
  `Passive High Pass Filter (Image electronics-tutorials) <https://www.electronics-tutorials.ws/filter/filter_3.html>`_

.. figure:: ./images/sig-hpf-lpf.png
  :align: center
  :scale: 80%

  `Green Curve is the original signal, red/blue are filtered signals after low pass filters, black is the filtered signal after a high pass filter (Image stackoverflow) <https://stackoverflow.com/questions/7105962/how-do-i-run-a-high-pass-or-low-pass-filter-on-data-points-in-r>`_

Filtering is a very common signal conditioning procedure (`learn more <https://www.electronics-tutorials.ws/category/filter>`_). There are many other signal conditioning techniques, but I will leave this topic open for you to explore.

Analog to Digital Conversion
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

After proper signal conditioning, the analog signal is sampled and converted to digital signal by an analog to digital converter (ADC). The following figure shows a resolution difference of a 3-bit and a 16-bit ADC. Note that ADC with higher resolution are increasing more expensive.

.. figure:: ./images/adc-resolution.png
  :align: center
  :scale: 50%

  `3-bit ADC (blue line) versus 16-bit ADC (red line) (Image ni.com) <https://learn.ni.com/teach/resources/945/adc-and-sampling>`_


Monitor and Record
^^^^^^^^^^^^^^^^^^

The converted digital signals can be transfered to a computing device such as a laptop to monitor and record. Generally, this procedure is done by a software interface between the DAQ harware and the computer system.

.. figure:: ./images/computer.png
  :align: center
  :scale: 50%

  `Monitor and Record Data (Image ni.com) <https://www.ni.com/en-us/shop/daqexpress.html>`_

.. toctree::
   :maxdepth: 1