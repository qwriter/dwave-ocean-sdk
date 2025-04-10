.. _opt_solver_cqm_properties:

=====================
CQM Solver Properties
=====================

This section describes the properties of quantum-classical hybrid
:ref:`constrained quadratic model <concept_models_cqm>` solvers such as the Leap
service's ``hybrid_constrained_quadratic_model_version1``. For the parameters
you can configure, see the :ref:`opt_solver_cqm_parameters` section.

.. _property_cqm_category:

category
========

.. include:: ../shared/properties.rst
    :start-after: start_property_category_hybrid
    :end-before: end_property_category_hybrid

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()    # doctest: +SKIP
>>> sampler.properties["category"]      # doctest: +SKIP
'hybrid'


.. _property_cqm_maximum_number_of_biases:

maximum_number_of_biases
========================

.. include:: ../shared/properties.rst
    :start-after: start_property_maximum_number_of_biases
    :end-before: end_property_maximum_number_of_biases

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                # doctest: +SKIP
>>> sampler.properties["maximum_number_of_biases"]  # doctest: +SKIP
750000000


.. _property_cqm_maximum_number_of_constraints:

maximum_number_of_constraints
=============================

Maximum number of constraints accepted by the solver.

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                        # doctest: +SKIP
>>> sampler.properties["maximum_number_of_constraints"]     # doctest: +SKIP
100000


.. _property_cqm_maximum_number_of_linear_biases_real:

maximum_number_of_linear_biases_real
====================================

Maximum number of linear biases of type floating-point/real numbers counted
across all constraints and the model's objective.

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                            # doctest: +SKIP
>>> sampler.properties["maximum_number_of_linear_biases_real"]  # doctest: +SKIP
75000000


.. _property_cqm_maximum_number_of_quadratic_variables:

maximum_number_of_quadratic_variables
=====================================

Maximum number of variables that have interactions (quadratic biases)---counted
across all constraints (meaning that the same variable can be counted multiple
times if it appears in interactions in more than one constraint)---accepted by
the solver.

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                            # doctest: +SKIP
>>> sampler.properties["maximum_number_of_quadratic_variables"] # doctest: +SKIP
15000000


.. _property_cqm_maximum_number_of_quadratic_variables_real:

maximum_number_of_quadratic_variables_real
==========================================

Maximum number of variables that have interactions (quadratic biases) of type
floating-point/real numbers---counted across all constraints (meaning that the
same variable can be counted multiple times if it appears in interactions in
more than one constraint)---accepted by the solver.

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                            # doctest: +SKIP
>>> sampler.properties["maximum_number_of_quadratic_variables_real"]   # doctest: +SKIP
0


.. _property_cqm_maximum_number_of_variables:

maximum_number_of_variables
===========================

.. include:: ../shared/properties.rst
    :start-after: start_property_maximum_number_of_variables
    :end-before: end_property_maximum_number_of_variables

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                    # doctest: +SKIP
>>> sampler.properties["maximum_number_of_variables"]   # doctest: +SKIP
5000000


.. _property_cqm_maximum_time_limit_hrs:

maximum_time_limit_hrs
======================

.. include:: ../shared/properties.rst
    :start-after: start_property_maximum_time_limit_hrs
    :end-before: end_property_maximum_time_limit_hrs

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                # doctest: +SKIP
>>> sampler.properties["maximum_time_limit_hrs"]    # doctest: +SKIP
24.0


.. _property_cqm_minimum_time_limit_s:

minimum_time_limit_s
====================

Minimum required run time, in seconds, the solver must be allowed to work on any
given problem.

For more details, see the :ref:`system_samplers` section for solver methods that
calculate the default runtime of a given problem.

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                # doctest: +SKIP
>>> sampler.properties["minimum_time_limit_s"]      # doctest: +SKIP
5


.. _property_cqm_num_biases_multiplier:

num_biases_multiplier
=====================

Multiplier used in the internal calculation of the minimum run time,
:ref:`property_cqm_minimum_time_limit_s`, the solver must be allowed to work on
the given problem.

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                    # doctest: +SKIP
>>> sampler.properties["num_biases_multiplier"]         # doctest: +SKIP
4.65705646e-06


.. _property_cqm_num_constraints_multiplier:

num_constraints_multiplier
==========================

Multiplier used in the internal calculation of the minimum run time,
:ref:`property_cqm_minimum_time_limit_s`, the solver must be allowed to work on
the given problem.

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                        # doctest: +SKIP
>>> sampler.properties["num_constraints_multiplier"]        # doctest: +SKIP
6.44385747e-09


.. _property_cqm_num_variables_multiplier:

num_variables_multiplier
========================

Multiplier used in the internal calculation of the minimum run time,
:ref:`property_cqm_minimum_time_limit_s`, the solver must be allowed to work on
the given problem.

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                        # doctest: +SKIP
>>> sampler.properties["num_variables_multiplier"]          # doctest: +SKIP
0.000157411458


.. _property_cqm_parameters:

parameters
==========

.. include:: ../shared/properties.rst
    :start-after: start_property_parameters
    :end-before: end_property_parameters

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                # doctest: +SKIP
>>> sampler.properties["parameters"]["time_limit"]  # doctest: +SKIP
'Maximum runtime, in seconds, requested for the problem submission.'


.. _property_cqm_quota_conversion_rate:

quota_conversion_rate
=====================

.. include:: ../shared/properties.rst
    :start-after: start_property_quota_conversion_rate
    :end-before: end_property_quota_conversion_rate

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                # doctest: +SKIP
>>> sampler.properties["quota_conversion_rate"]     # doctest: +SKIP
20


.. _property_cqm_supported_problem_types:

supported_problem_types
=======================

.. include:: ../shared/properties.rst
    :start-after: start_property_supported_problem_types
    :end-before: end_property_supported_problem_types

CQM solvers support the following energy-minimization problem types:

*   ``cqm``

    .. include:: ../shared/models.rst
        :start-after: start_models_cqm
        :end-before: end_models_cqm

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()                # doctest: +SKIP
>>> sampler.properties["supported_problem_types"]   # doctest: +SKIP
['cqm']


.. _property_cqm_version:

version
=======

.. include:: ../shared/properties.rst
    :start-after: start_property_version
    :end-before: end_property_version

Example
-------

>>> from dwave.system import LeapHybridCQMSampler
...
>>> sampler = LeapHybridCQMSampler()    # doctest: +SKIP
>>> sampler.properties["version"]       # doctest: +SKIP
1.12