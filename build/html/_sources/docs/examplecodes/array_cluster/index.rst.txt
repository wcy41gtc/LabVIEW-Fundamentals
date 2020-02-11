.. _array_cluster_index:

Example Code: Arrays. Clusters and Data Bundling
================================================

Overview
^^^^^^^^

This example VI demonstrates basics of arrays, clusters, and how to bundle data in a cluster with or without name(label).

.. figure:: array_cluster_bundle_front_panel.png
  :align: center
  :scale: 60%

  `Front panel of arrays_clusters_bundles.vi`

.. figure:: array_cluster_bundle_block_diagram.png
  :align: center
  :scale: 60%

  `Block diagram of arrays_clusters_bundles.vi`

Behavior
^^^^^^^^

#. 1-D Array

   If array elements are initialized in the 1-D array control, they are pssed to the 1-D array indicator.

#. 2-D Array

   Specify the inital value, rows, and columns, the 2-D array indicator should show the initialized array correspondingly.

#. Extract Array Subset

   Specify the starting index and the range for the row and column in the predefined array, the array indcator should show extracted subset/elemensts.

#. Bundle a numerical value, a boolean value and a string into a cluster without labels.

#. Bundle a numerical value, a boolean value and a string into a cluster with labels, and extract the elements in the cluster by its label.


:download:`arrays_clusters_bundles.vi <arrays_clusters_bundles.vi>`

