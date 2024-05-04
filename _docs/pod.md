---
layout: docs
title:  "Pod"
sections:
  - Example
#  - Why do we need to work together
---

A slice of a node that provides a layer of abstraction for defining a scoped piece of work, including (but not limited to) providing an operating system, or a grouping of resources. A pod typically makes a request for resources, and is intended to run one or more units of work (e.g., containers). Pods are exclusive to Kubernetes and the term is not used in HPC, however we might consider the HPC equivalent to be anything that represents a "unit of computing" that is schedulable for units of work (some number of containers or applications).

## Example

For Kubernetes, a unit of computing is referred to as a Pod, which explicitly is a group of containers with shared storage and network resources. A pod is a logical node. It is the smallest unit of work you can deploy. The closest thing we have in HPC would be like a scheduling script or a resource request - a packaged set of work that requires some set of resources. A key difference is that pods are designed to well support services, while batch work on HPC is not.
