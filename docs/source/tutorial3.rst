Tutorial-3
~~~~~~~~~~

Importing the package
^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    import nz_seqtech


Importing classical_ml_models class and functions
^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    from nz_seqtech.classical_ml_models import gaussian_process_model, decision_tree_model, suggested_dataset1

Testing gaussian_process_model with a suggested dataset
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    gaussian_process_model(suggested_data=True)


.. parsed-literal::

                  precision    recall  f1-score   support
    
               0       1.00      0.82      0.90        17
               1       0.77      1.00      0.87        10
    
        accuracy                           0.89        27
       macro avg       0.88      0.91      0.89        27
    weighted avg       0.91      0.89      0.89        27
    


Testing decision_tree_model with a loaded dataset
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: ipython3

    # Load data from npy files 
    X_train = numpy.load('x_train.npy')
    X_test = numpy.load('x_test.npy')
    Y_train = numpy.load('y_train.npy')
    Y_test = numpy.load('y_test.npy')
    
    decision_tree_model(X_train,X_test,Y_train,Y_test,suggested_data=False)


.. parsed-literal::

                  precision    recall  f1-score   support
    
               0       0.50      0.33      0.40         6
               1       0.75      0.86      0.80        14
    
        accuracy                           0.70        20
       macro avg       0.62      0.60      0.60        20
    weighted avg       0.68      0.70      0.68        20
    

