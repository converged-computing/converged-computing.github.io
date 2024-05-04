---
layout: docs
title:  "Scheduling"
sections:
  - Example
---

Taking a resource request and performing a mapping such that units of work are mapped to resources. A scheduler is a function that takes as input a triple (resource shape, requested start time, requested time interval) and outputs a four tuple (resources, start time of guarantee, end time guarantee, binding guarantee) to map the units of work to said resources. For a graph scheduler, this means that a job is translated to a resource request, and the resource request is a subgraph of the entire graph of resources known to the scheduler. If it's the case that a subgraph is mapped to a job id because of a reservation, we search a smaller search space. The unit of time is a variable here, as different schedulers will honor different units.

## Example

In Kubernetes, “scheduling” is the finding a node that can satisfy your resource request. Unlike in HPC, it is specific to scheduling pods (resource groups with containers) to physical nodes. In simple terms - "What runs next and where."
