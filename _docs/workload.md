---
layout: docs
title:  "Workload"
#sections:
#  - What is Converged Computing
#  - Why do we need to work together
---

A workload is a set of jobs or tasks scheduled by a scheduler and managed by a resource manager.  In the simplest terms, it could be as a single job tasked to do some computation using a defined set of resources. In more realistic terms, it is a data-intensive task that is spread across nodes and runs in parallel where each part uses a subset of CPU/GPU. A workload is not a workflow that has a directed acyclic graph (DAG) but rather the units of work in the graph. A vertex in a workflow DAG is a workload. If you find yourself saying Step A THEN B, you likely are not in a workload (step) but thinking about a workflow (DAG).
