.. _config_cluster_manager_cluster_circuit_breakers:

Circuit breaking
================

* Circuit Breaking :ref:`architecture overview <arch_overview_circuit_break>`.
* :ref:`v2 API documentation <envoy_api_msg_cluster.CircuitBreakers>`.

Runtime
-------

All circuit breaking settings are runtime configurable for all defined priorities based on cluster
name. They follow the following naming scheme ``circuit_breakers.<cluster_name>.<priority>.<setting>``.
``cluster_name`` is the name field in each cluster's configuration, which is set in the Envoy
:ref:`config file <envoy_api_field_Cluster.name>`. Available runtime settings will override
settings set in the Envoy config file.
