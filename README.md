# Test Driven Developments(TDD) in PySpark

Why TDD for PySpark?

TDD enables properly designing the test cases before writing the actual code and helps us validate the expected output. It provides us an opportunity to write robust code with well-rounded tests.

How to Implement?

Arrange —> Act —> Assert Pattern

Example: Write a PySpark program to split words for the text content in the wikipedia page - 'Test Driven Development(https://lnkd.in/gpu9du48)'

# Arrange: 1. input and expected dataframes for the method and 2. input and expected schemas.

# Act: Call the function we are testing by passing the input dataframe created in the Arrange step.

# Assert: Compare the actual and expected values. In this case, the dataframe values and schema.

# Developments:

First Inference: Define function structure
Second Inference: Write logic to split input string

Executing the test now will fail and we need to refactor more as split function returns the output in the form of array, but we need each word to be part of a separate row.

Third Inference: Refactor logic to return each word in a separate row.

Great ! The test passed successfully. We have followed the TDD approach to define the test and then, refactored the function to pass the test.
