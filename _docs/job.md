---
layout: docs
title:  "Job"
#sections:
#  - What is Converged Computing
#  - Why do we need to work together
---

A job is a unit of work that runs to completion, and is typically the combination of input data, environment variables, description of resources needed, an application, and output directives. On a high level a single job can be replicated into an array (multiple of the same job run in parallel) or assembled like legos into a workflow to manifest in more complex application logic. It's common to refer to a grouping of jobs, where they are non-interactive and submitting to use a complex set of resources, as a batch job.  A job is typically akin to one step or task in a workflow, or run on its own.

{% include example.html text="In Flux, a batch job can be defined by way of a script that can create one or more flux jobs or even allocations. In Kubernetes, a batch job could be a Job, or a JobSet." %}