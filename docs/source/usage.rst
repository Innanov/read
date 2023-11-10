NZ-SeQTech Documentation
========================

Installation
------------

To use NZ-SeQTech, first install it using pip:

.. code-block:: python

    !pip install nz-seqtech

Quantum DNA Encoding
--------------------

You can encode DNA sequences using various techniques provided by NZ-SeQTech's `quantum_dna_encoding` module. Here's an example of how to use the `cosine_encoding` function:

.. code-block:: python

   import nz_seqtech
   from nz_seqtech.quantum_dna_encoding import cosine_encoding

   # Encode DNA sequence using cosine encoding
   encoded_sequence = cosine_encoding('sequence')
   print(encoded_sequence)

This example imports the necessary module and function, then uses `cosine_encoding` to encode a DNA sequence. The resulting encoded sequence is stored in the `encoded_sequence` variable.

When using the function, make sure to replace `'sequence'` with your actual DNA sequence.

For more encoding techniques and visualization functions, you can explore other functions in the `quantum_dna_encoding` module:

- `amplitude_encoding`
- `qft_encoding`
- `phase_encoding`
- `NZ23_encoding`
- `NZ22_encoding`
- `draw_circuit`
- `get_statevector`
- `visualize_bloch_multivector`
- `visualize_state_hinton`
- `visualize_state_city`
- `visualize_state_paulivec`

Refer to the documentation or use the `help` function for each specific function to learn more about its parameters and usage.

Classical DNA Sequence Analysis
-------------------------------

You can also perform classical DNA sequence analysis using functions from the `classical_operations` module. For example:

.. code-block:: python

   import nz_seqtech
   from nz_seqtech.classical_operations import analyze_dna_seq

   # Analyze DNA sequence
   analysis_result = analyze_dna_seq('sequence')
   print(analysis_result)

Replace `'sequence'` with your actual DNA sequence when using the function.

Classical Machine Learning Models
----------------------------------

NZ-SeQTech provides classical machine learning models that you can use for DNA sequence analysis. Import the desired model from the `classical_ml_models` module and follow the usage examples provided in the documentation for each specific model.

.. code-block:: python

   import nz_seqtech
   from nz_seqtech.classical_ml_models import knn_model

   # Create and train a k-nearest neighbors model
   model = knn_model(X_train, X_test, y_train, y_test, suggested_data=True)

Replace `X_train` , `X_test` , `y_train` and `y_test` with your actual data.


Quantum Machine Learning Models
----------------------------------
If you are interested in quantum machine learning, you can explore the quantum machine learning models provided by NZ-SeQTech in the quantum_ml_models module. Follow the usage examples in the documentation for each specific model.

.. code-block:: python

   import nz_seqtech
   from nz_seqtech.classical_ml_models import QNN

   # Create and train a Quantum Neural Network (QNN) model
   qnn_model = QNN(X, y, suggested_data=True)

Replace `X` and `y` with your actual data.

Note: The `suggested_data` parameter is set to `True` to indicate using the provided datasets in the package for testing. If you prefer to use your own data, set `suggested_data` to `False` and provide your training and testing data.
