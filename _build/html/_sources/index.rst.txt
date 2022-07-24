Improve bizstyle
===============================================

.. contents::
  :depth: 2
  :local:
  :backlinks: entry

line block
----------

.. code-block:: rst

  .. note::
      | test
      | test

.. code-block:: css

  div.admonition div.line-block {
    margin: 0.5em 1em 0.5em 1em;
  }

.. note::
  | test
  | test

admonition+table
----------------

.. code-block:: rst

  .. note::
    .. list-table::

      * - abc
        - def
        - efg
      * - abc
        - def
        - efg

.. code-block:: css

  div.admonition table {
    margin: 0.5em 1em 0.5em 1em;
  }


.. note::
  .. list-table::

    * - abc
      - def
      - efg
    * - abc
      - def
      - efg

table
-----

code rst
~~~~~~~~

.. code-block:: rst

  .. list-table::
      :header-rows: 1

    * - hoge
    - fuga
    * - hoge
      - + fuga
        + fuga2

code css
~~~~~~~~

.. code-block:: css

  td ul.simple {
    padding-left: 20px;
  }

before
~~~~~~

.. figure:: _static/table.png


after
~~~~~

.. list-table::
  :header-rows: 1

  * - hoge
    - fuga
  * - hoge
    - + fuga
      + fuga2

[TODO] code-block caption
-------------------------

.. code-block:: rst

  .. code-block:: rst
    :caption: caption

    hoge
    ====

.. code-block:: rst
  :caption: caption

  hoge
  ====

