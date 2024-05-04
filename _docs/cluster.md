---
layout: docs
title:  "Cluster"
sections:
  - Example
---

A cluster is a group of resources that collectively run applications or provide services or storage. Clusters exist to serve the needs of multiple users and/or multiple applications with resource requirements that are greater than what is provided by a single machine. The complexity of the cluster generally reflects the needs of its users, and often reflects the economic decisions of a center providing the resource.

## Example

As an example, owning a cluster (common in HPC communities) presents a different cost model than renting resources (common for cloud) that providers/centers must choose between. The nodes can be co-located (close by in terms of communication latency) or far apart (regions or zones in a cloud provider). Generally speaking, co-location can have a huge influence on network latency and thus application performance. If we consider all the compute in the world, we can consider a cluster akin to a cluster in a graph - a set of vertices that are more highly connected to one another than other nodes. A cluster could be a set of nodes running a resource manager on bare metal of an HPC cluster, or a set of nodes running Kubernetes and applications via pods on those nodes. While cloud and HPC are predominant now, the first distributed clusters came by way of grid computing in the early 1990s.
