---
layout: docs
title:  "Nodes"
sections:
  - Example
---

> Synonyms: virtual machine (VM) instances, server

A node is a server resource, an addressable compute or storage unit (often supporting an ip-address). A node can either be:

- virtual: an abstraction to virtualize system resources. A node that is virtual can be a virtual machine, which uses some hypervisor technology, or even a linux container. 
- physical: no virtualization, and often called "bare metal"

A node can exclusively be for storage or compute, or can serve both purposes. 

## Example

A [Kubernetes node](https://kubernetes.io/docs/concepts/architecture/nodes/) is typically intended for compute, as the unit for storage would be called a [volume](https://kubernetes.io/docs/concepts/storage/). A node deployed for HPC typically takes on one role or a hybrid approach. Nodes can be shared or exclusive (see allocation type). At a high level, a "node" might refer to an instance on a cloud provider, a "node" in Kubernetes [[ref](https://kubernetes.io/docs/concepts/architecture/nodes/)], or a bare metal machine. It is an abstraction for a base machine.
