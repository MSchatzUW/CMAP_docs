.. _dataViz:



Data Visualization
==================

.. _plotly: https://plot.ly/
.. _bokeh: https://bokeh.pydata.org/en/latest/index.html
.. _API: pycmap_api.html
.. _API key: pycmap_api.html


.. image:: https://colab.research.google.com/assets/colab-badge.svg
   :target: https://colab.research.google.com/github/simonscmap/pycmap/blob/master/docs/Viz.ipynb

.. image:: https://mybinder.org/badge_logo.svg
   :target: https://mybinder.org/v2/gh/simonscmap/pycmap/master?filepath=docs%2FViz.ipynb



The main focus of pycmap (and the broader Simons CMAP project) is to
provide the user with a unifying API to extract subsets of datasets with
different dimensions and different spatio-temporal resolutions. This
will drastically reduce the time-consuming data collection and
preparation processes, especially considering the massive size of the
archived multi-decade global oceanic datasets generated by satellites or
numerical models.

The simple and unified interface of the pycmap API enables the general
public and scientists to dive into the vast, and often under
underutilized, ocean datasets without being concerned about the
underlying dataset file structure. Visualizing the retrieved data is
often a good entry point to explore and study these datasets and pycmap
offers a number of builtin methods for simple interactive data
visualizations. The pycmap visualizetion engine can be set to either of
these interactive data visualization libraries: `plotly`_, or `bokeh`_.
Plotly has a larger variation graphs while bokeh is faster to render the
graph object.

The default visualization library is plotly; the code block below shows
how to change the visualization engine (see `API`_ page for more
details).

.. note::

  Data visualization requires a valid `API key`_ which can be obtained
  from https://simonscmap.com/. It is not necessary to set the API key
  every time because the API properties are stored locally after being
  called the first time.




**Example**

.. code-block:: python

  import pycmap
  pycmap.API(vizEngine='bokeh')  # vizEngine options: 'plotly' ,'bokeh'



Data Visualization Methods
--------------------------


+-------------------------------+--------------------------------------------------------------+
| :ref:`histogram`              |       Histogram Plot                                         |
+-------------------------------+--------------------------------------------------------------+
| :ref:`timeSeries`             |       Time Series Plot                                       |
+-------------------------------+--------------------------------------------------------------+
| :ref:`rmCp3d`                 |       Regional Map, Contour Plot, 3D Surface Plot            |
+-------------------------------+--------------------------------------------------------------+
| :ref:`sectionMapContour`      |       Section Map, Section Contour                           |
+-------------------------------+--------------------------------------------------------------+
| :ref:`depthProfile`           | Depth Profile                                                |
+-------------------------------+--------------------------------------------------------------+
| :ref:`cruiseTrackPlot`        | Cruise Track Plot                                            |
+-------------------------------+--------------------------------------------------------------+
| :ref:`corrMatrix`             | Correlation Matrix                                           |
+-------------------------------+--------------------------------------------------------------+
| :ref:`corrMatrixCruise`       | Correlation Matrix Along Cruise Track                        |
+-------------------------------+--------------------------------------------------------------+



.. toctree::
  :maxdepth: 1
  :hidden:

  data_vizualization/pycmap_histogram
  data_vizualization/pycmap_time_series
  data_vizualization/pycmap_rm_cp_3d
  data_vizualization/pycmap_section_map_contour
  data_vizualization/pycmap_depth_profile
  data_vizualization/pycmap_cruise_track
  data_vizualization/pycmap_correlation_matrix
  data_vizualization/pycmap_correlation_matrix_cruise_track
