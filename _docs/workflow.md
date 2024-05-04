---
layout: docs
title:  "Workflow"
#sections:
#  - What is Converged Computing
#  - Why do we need to work together
---

A workflow is a set of tasks with dependencies that need to be executed in a specific order for proper handling of exchanging inputs and outputs of data. Workflows typically have two components: data and applications, and workflow tools must decide the granularity at which to map tasks to execution workload units.  Workflow steps can map into workloads, e.g.,

```
workflow -> DAG -> scheduler -> workload
```

{% include example.html prefix="" text="A workflow tool might generate a directed acyclic graph (DAG) of individual tasks that can be handed to a scheduler." %} 


