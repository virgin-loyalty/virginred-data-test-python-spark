# Coding Test - Data Engineering - Spark

This test is based on the following:

- https://github.com/JSainsburyPLC/aspire-data-test-python
- https://github.com/infinityworks/iw-data-test-python

# Prerequisites

To run this test, you will need an environment suitable for PySpark >= 3.1, with the former
requiring Java 8 or 11. It is part of the test that you are able to set this up on your own.

Some initial dependencies are available in `requirements.txt`. Note that depending on your version of Python, PySpark,
and Java, PySpark might fail to install unless you first install `pypandoc`. It is recommended that you use a
virtual environment.

We recommend using an IDE. At Virgin Red, the most common product is PyCharm, the Community Edition of which
may be downloaded for free [here](https://www.jetbrains.com/pycharm/download/#section=mac).

# Running tests

```bash
pytest ./tests
```

# Generating the data

A data generator is included as part of the project in `./input_data_generator/main_data_generator.py`
This allows you to generate a configurable number of months of data.
Although the technical test specification mentions 6 months of data, it's best to generate
less than that initially to help improve the debugging process.

To run the data generator use:

```bash
python ./input_data_generator/main_data_generator.py
```

This will produce customer, product, and transaction data at `./input_data/starter`

# Getting started

The skeleton of a possible solution is provided in `./solution/solution_start.py`, but you do not have to use this code.
Re-organise this repository as best you see fit to approach the problems stated in the way you find preferable and
most appropriate.
