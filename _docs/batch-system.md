---
layout: docs
title:  "Batch System"
#sections:
#  - What is Converged Computing
#  - Why do we need to work together
---

A batch system provides the interface to manage resources and schedule workloads. Due to the complexity, batch systems often manifest as a combination of components or modules, and we can see this for both HPC systems and Kubernetes.

Advanced / developer note: the modularity afforded by these systems often makes them very flexible / pluggable for integrating components from one into the other, etc. Batch systems can be nested in other batch systems, if the technology allows for it.


{% include example.html prefix="Flux:" text="We might consider the combination of flux-core, flux-sched, and flux-security as a combined set of modules that manifest in a batch system, deployed on either bare metal or a virtual machine (or pod)." %}

<br>

{% include example.html prefix="Kubernetes:" text="We might consider the Kubernetes default scheduler combined with control-plane(s) and one or more kubelet a basic batch system, with the addition of Kueue to add a queue. In both cases, the batch systems can receive some specification for a unit of work (e.g., a job)." %}
