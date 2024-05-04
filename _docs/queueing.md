---
layout: docs
title:  "Scheduling"
sections:
  - Example
---

A means to take requests for work and order them in a way by priority (fair share or other algorithms) and availability. Queuing systems are interested in attributes such as satisfiability, reservations, and backfilling. 

## Example

In Kubernetes, a tool like Kueue [[ref](https://kueue.sigs.k8s.io/docs/tasks/administer_cluster_quotas/)] might create simple job requests for users and assign them to be run based on priority settings. In an HPC resource manager like SLURM [[ref](https://slurm.schedmd.com/quickstart.html)], it's more likely that groups of nodes (called partitions) are allocated to user jobs based on an algorithm like fair share.

