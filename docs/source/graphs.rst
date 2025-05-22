Graph Visualization
===================

``ezmsg`` can export the topology of a running pipeline as either a Graphviz or
Mermaid diagram. These features are exposed through the command line
interface.

Using ``ezmsg graphviz``
------------------------

Run ``ezmsg graphviz`` while a pipeline is running to print a Graphviz ``dot``
representation of the current graph.
You can redirect this output to a file and then render it with Graphviz tools::

  ezmsg graphviz > pipeline.dot
  dot -Tpng pipeline.dot -o pipeline.png

Using ``ezmsg mermaid``
-----------------------

The ``ezmsg mermaid`` command prints a Mermaid diagram. By default it will open
an online viewer so that the graph is rendered in the browser. The output can
also be redirected to a file or encoded for `mermaid.ink` or other targets using
the ``--target`` option.

Example::

  ezmsg mermaid --target live

This will open `https://mermaid.live` with the diagram pre-loaded. Valid targets
are ``ink`` (for mermaid.ink), ``live`` (default), and ``play`` (mermaidchart.com).

