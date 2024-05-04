---
layout: docs
title:  "Resources"
sections:
  - Example
---


Hardware (nodes, storage, accelerators) or flow transports (network, power) that make up a system (that can be logically partitioned for tasks) and can be consumed by its users. Each resource type has a unit of abstraction, and is finite and thus needs to be managed.


## Example

Hardware typically provides compute or storage for a job, and the scale can vary from a socket or CPU to an entire node. The finite nature of resources in the context of some number of tasks or users requires intelligent scheduling. On cloud, there is a perception that resources are unlimited, and only bounded by the amount of money allowed to be spent. This is typically not the truth. For high performance computing, the entire set of resources is more transparent. In both cases, the resources are finite, however the perception is different.

