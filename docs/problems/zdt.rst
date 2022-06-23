ZDT 
========

The ZDT problem suite is based on the construction process:

.. math::

  \min && \; f_1(x) && \;\\[2mm]
  \min && \; f_2(x) && \;= g(x) \, h(f_1(x),g(x))

where two objective have to be minimized. The function :math:`g(x)` can be considered as the function for convergenece and usually :math:`g(x)=1` holds for pareto-optimal solutions (except for ZDT5).

More details about the test problems can be found in [Zitzler2000]_ 


ZDT1
----
This is a 30-variable problem (:math:`n=30`) with a convex Pareto-optimal set:


**Definition**

.. math::

  f_1(x) &= \, & x_1 \\
  g(x) &=& 1 + \frac{9}{n-1} \; \sum_{i=2}^{n} x_i \\
  h(f_1,g) &=& 1 - \sqrt{f_1/g} \\

**Optimum**

.. math::

  && \;0 \leq x_1^* \leq 1  \quad \text{and} \quad x_i^*=0 \; \text{for} \; i=2,\ldots,n\\


ZDT2
----
This is also a 30-variable problem (:math:`n=30`) with a non-convex Pareto-optimal set:

**Definition**

.. math::

  f_1(x) &= \, & x_1 \\
  g(x) &=& 1 + \frac{9}{n-1} \; \sum_{i=2}^{n} x_i \\
  h(f_1,g) &=& 1 - (f_1/g)^2 \\


**Optimum**

.. math::
  0 \leq x_1^* \leq 1  \quad \text{and} \quad x_i^*=0 \; \text{for} \; i=2,\ldots,n


ZDT3
----

ZDT4
----

ZDT5
----

ZDT6
----


.. [Zitzler2000] Eckart Zitzler, Kalyanmoy Deb, and Lothar Thiele. Comparison of multiobjective evolutionary algorithms: empirical results. Evolutionary Computation, 8(2):173–195, 2000. doi:10.1162/106365600568202.