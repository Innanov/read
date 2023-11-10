Tutorial-2
~~~~~~~~~~

Importing the package
^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    import nz_seqtech

Importing classical_operations module
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    from nz_seqtech.classical_operations import analyze_dna_seq

Testing the DNA analyser
^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    dna='AGTCcgA'

.. code:: ipython3

    analyze_dna_seq(dna)




.. parsed-literal::

    ({'A': 2, 'T': 1, 'G': 2, 'C': 2},
     {'A': 0.2857142857142857,
      'T': 0.14285714285714285,
      'G': 0.2857142857142857,
      'C': 0.2857142857142857},
     0.1875,
     0.4330127018922193,
     array(0.25),
     1.0,
     -1.1547005383792515,
     -0.6666666666666665)




.. image:: output_7_1.png



.. image:: output_7_2.png



.. image:: output_7_3.png

