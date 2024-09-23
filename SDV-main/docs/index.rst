|Development Status| |PyPi Shield| |Run Tests| |Coverage Status|
|Downloads| |Binder| |Slack|

.. raw:: html

    <p align="center">
    <a href="https://github.com/sdv-dev/SDV">
    <img align="center" width=40% src="_static/SDV-DataCebo.png"></img>
    </a>
    </p>

========================

**Date**: |today| **Version**: 0.18.0

Overview
--------

The **Synthetic Data Vault (SDV)** is a **Synthetic Data Generation**
ecosystem of libraries that allows users to easily learn :ref:`single-table
<single_table>`, :ref:`multi-table <relational>` and :ref:`timeseries <timeseries>`
datasets to later on generate new **Synthetic Data** that has the **same format and
statistical properties** as the original dataset.

Synthetic data can then be used to supplement, augment and in some cases
replace real data when training Machine Learning models. Additionally,
it enables the testing of Machine Learning or other data dependent
software systems without the risk of exposure that comes with data
disclosure.

Underneath the hood it uses several probabilistic graphical modeling and
deep learning based techniques. To enable a variety of data storage
structures, we employ unique hierarchical generative modeling and
recursive sampling techniques.

Current functionality and features:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-  Synthetic data generators for :ref:`single table datasets <single_table>` with the following
   features:

   -  Using :ref:`Copulas <gaussian_copula>` and :ref:`Deep Learning <ctgan>` based models.
   -  Handling of multiple data types and missing data with minimum user input.
   -  Support for :ref:`pre-defined and custom constraints <single_table_constraints>` and data
      validation.

-  Synthetic data generators for :ref:`complex, multi-table, relational datasets <relational>`
   with the following features:

   -  Definition of entire :ref:`multi-table datasets metadata <relational_metadata>` with a custom
      and flexible :ref:`JSON schema <metadata_schema>`.
   -  Using Copulas and recursive modeling techniques.

-  Synthetic data generators for :ref:`multi-type, multi-variate timeseries datasets <timeseries>`
   with the following features:

   -  Using statistical, Autoregressive and Deep Learning models.
   -  Conditional sampling based on contextual attributes.

-  Metrics for :ref:`evaluation`, including:

   -  An easy to use :ref:`evaluation_framework` to evaluate the quality of your synthetic
      data with a single line of code.
   -  Metrics for multiple data modalities, including :ref:`single_table_metrics` and
      :ref:`multi_table_metrics`.

-  A :ref:`benchmarking_framework` to easily compare multiple synthetic data generators, including:

   -  Dozens of datasets of multiple data modalities already prepared to be run on.
   -  Tools to easily add new synthetic data generators and datasets.
   -  Distributed computing to reduce computing times.
   -  Comprehensive results presented in multiple leaderboard formats.

Try it out now!
---------------

If you want to quickly discover **SDV**, simply click the button below
and follow the tutorials!

|Binder|

Join our Slack Workspace
------------------------

If you want to be part of the SDV community to receive announcements of the latest releases,
ask questions, suggest new features or participate in the development meetings, please join
our Slack Workspace!

|Slack|

Explore SDV
-----------

* `Getting Started <getting_started/index.html>`_
* `User Guides <user_guides/index.html>`_
* `API Reference <api_reference/index.html>`_
* `Developer Guides <developer_guides/index.html>`_
* `Release Notes <history.html>`_

--------------

.. raw:: html

    <div align="center">
    <a href="https://datacebo.com"><img align="center" width=40% src="_static/DataCebo.png"></img></a>
    </div>
    <br/>
    <br/>

`The Synthetic Data Vault Project <https://sdv.dev>`_  was first created at MIT's `Data to AI Lab
<https://dai.lids.mit.edu/>`_ in 2016. After 4 years of research and traction with enterprise, we
created `DataCebo <https://datacebo.com>`_ in 2020 with the goal of growing the project.
Today, DataCebo is the proud developer of SDV, the largest ecosystem for synthetic data generation
& evaluation. It is home to multiple libraries that support synthetic data, including:

* 🔄 Data discovery & transformation. Reverse the transforms to reproduce realistic data.
* 🧠 Multiple machine learning models -- ranging from Copulas to Deep Learning -- to create tabular,
  multi table and time series data.
* 📊 Measuring quality and privacy of synthetic data, and comparing different synthetic data
  generation models.

`Get started using the SDV package <https://sdv.dev/SDV/getting_started/install.html>`_ -- a fully
integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
for specific needs.

--------------

.. |Development Status| image:: https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow
   :target: https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha
.. |PyPi Shield| image:: https://img.shields.io/pypi/v/SDV.svg
   :target: https://pypi.python.org/pypi/SDV
.. |Run Tests| image:: https://github.com/sdv-dev/SDV/workflows/Run%20Tests/badge.svg
   :target: https://github.com/sdv-dev/SDV/actions?query=workflow%3A%22Run+Tests%22+branch%3Amain
.. |Coverage Status| image:: https://codecov.io/gh/sdv-dev/SDV/branch/main/graph/badge.svg
   :target: https://codecov.io/gh/sdv-dev/SDV
.. |Downloads| image:: https://pepy.tech/badge/sdv
   :target: https://pepy.tech/project/sdv
.. |Binder| image:: https://mybinder.org/badge_logo.svg
   :target: https://mybinder.org/v2/gh/sdv-dev/SDV/main?filepath=tutorials
.. |Slack| image:: https://img.shields.io/badge/Slack%20Workspace-Join%20now!-36C5F0?logo=slack
   :target: https://bit.ly/sdv-slack-invite


.. toctree::
    :maxdepth: 3
    :hidden:
    :titlesonly:

    getting_started/index
    user_guides/index
    api_reference/index
    developer_guides/index
    Release Notes <history>
