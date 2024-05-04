---
layout: docs
title:  "Allocation"
#sections:
#  - Example
---

The actual set of physical resources that an application is running on. There are two types of allocations: shared and exclusive.

 - *Exclusive allocation*: jobs have dedicated physical resources (e.g., nodes, cores, memory). Multiple users cannot share a physical resource, and resources are not shared between jobs. This setup is common in HPC.
 - *Shared allocation*: jobs share underlying physical resources (e.g., nodes, cores, memory). Multiple users can run on the same physical resources. This setup is common in cloud.

