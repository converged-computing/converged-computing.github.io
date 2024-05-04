---
layout: docs
title:  "Batch"
#sections:
#  - What is Converged Computing
#  - Why do we need to work together
---

When someone says "batch" they are very generally referring to the combined system to manage resources and schedule workloads. The root of the term originates from "batch processing" - a sequence of programs and input data that would be processed in serial on a computer [[ref](https://en.wikipedia.org/wiki/Batch_processing)]. In Kubernetes, batch refers to the [working group](https://github.com/kubernetes/community/blob/master/wg-batch/README.md) and set of APIs (Job and CronJob abstractions) concerned with submitting jobs, which are fundamentally different than other Kubernetes objects because they have state, and are intended to be created and at some point complete. There is also a Cloud Native Compuing Foundation (CNCF) [batch working group](https://tag-runtime.cncf.io/wgs/bsi/charter/) that is interested in similar abstractions, and takes a stronger research standpoint. A very simple idea of "batch" (often used in Kubernetes) is to describe jobs running in parallel. This can be done both for Kubernetes and HPC. However, the coupling of the jobs is often very different between the spaces, with HPC being tightly coupled and Kubernetes batch more loosely. These ideas can be further expanded later.
