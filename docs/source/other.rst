Other ways to use ``ezmsg``
===========================

Command Line Interface
----------------------

The ``ezmsg`` command line interface exposes extra tools to manage a pipeline that is running in the background on a machine. Run ``ezmsg -h`` to see all the available options.

Graph Visualization with Graphviz and Mermaid
---------------------------------------------

You can inspect the connections of a running pipeline using the ``ezmsg graphviz``
and ``ezmsg mermaid`` commands. See :doc:`graphs` for details on generating and
viewing these diagrams.

Connecting Two ``ezmsg`` Pipelines
----------------------------------

Still under construction!

Notebooks
---------

An ezmsg pipeline can be run in a notebook environment with an extra parameter. When using ``run()``, include the optional kwarg ``force_single_process=True``.