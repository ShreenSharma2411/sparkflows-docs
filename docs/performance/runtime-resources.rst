Executor Memory, vcores
=======================

When running Apache Spark jobs, we can define the number of executors, executor memory and number of vcores per executor.

Normally dynamic allocation of executors is enabled, and we do not need to specify the number of executors.

Certain jobs need higher executor memory and number of vcores. These can be specified with ``--executor-memory`` and ``--executor-vcores``.

These additional spark configs can be specified in Fire in the Execute page. They can also be specified when the jobs are scheduled for execution.

