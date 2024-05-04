---
layout: docs
title:  "HPC vs HTC"
#sections:
#  - What is Converged Computing
#  - Why do we need to work together
---

Although HPC is mentioned heavily within k8s-batch, HTC is not covered as extensively. 

HPC, or "High Performance Computing," refers to the deployment and use of supercomputers and parallel processing techniques for solving complex computational problems. HPC systems are designed to deliver high performance by aggregating computing power in a way that enables higher processing speed and throughput for tasks that require significant computational resources.

Whereas HTC, or "High Throughput Computing," focuses on the efficient execution of a large number of loosely coupled or independent tasks over long periods of time. HTC systems are optimized not for the raw speed of any single computation, but for the overall volume of computations that can be performed over a given time period. 

K8s is not constructed for HTC workloads, and there are [no plans to support it natively](https://github.com/kubernetes-sigs/kueue/blob/main/keps/693-multikueue/README.md?plain=1#L56). The main players trying to support k8s-HTC are [HTCondor](https://htcondor.org/) (both in k8s and out) as well as [Armada](https://github.com/armadaproject/armada). 

There is also MTC, “Many Task Computing”, which tries to bridge the two, but that term is used significantly less. See these [notes](https://en.wikipedia.org/wiki/High-throughput_computing#High-throughput_vs._high-performance_vs._many-task) on Wikipedia to learn more.
