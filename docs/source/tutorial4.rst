Tutorial-4
================

Importing the package
^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    import nz_seqtech

Importing quantum_ml_models module
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    import nz_seqtech.quantum_ml_models

Importing QNN class
^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    from nz_seqtech.quantum_ml_models import QNN

Testing QNN class with a suggested dataset
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    QNN(suggested_data=True)



.. image:: figures/output_9_0.png


.. parsed-literal::

    Classification Report:
                   precision    recall  f1-score   support
    
              -1       0.47      0.73      0.57        11
               1       0.62      0.36      0.45        14
    
        accuracy                           0.52        25
       macro avg       0.55      0.54      0.51        25
    weighted avg       0.56      0.52      0.51        25
    


Testing QNN class with a loaded dataset
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    # Load data from X.npy and assign it to variable X
    X = numpy.load('x1.npy')
    
    # Load data from Y.npy and assign it to variable Y
    Y = numpy.load('y1.npy')
    
    QNN(X,Y,suggested_data=False)



.. image:: figures/output_11_0.png


.. parsed-literal::

    Classification Report:
                   precision    recall  f1-score   support
    
               0       0.00      0.00      0.00         9
               1       0.64      1.00      0.78        16
    
        accuracy                           0.64        25
       macro avg       0.32      0.50      0.39        25
    weighted avg       0.41      0.64      0.50        25
    

