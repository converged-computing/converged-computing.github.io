---
layout: docs
title:  "Job Specification"
#sections:
#  - Example
---

An abstraction that describes the resources, applications, task configuration, and amount of time needed by a job. This includes (on a high level) everything from executables to environment to resources needed. In Kubernetes a jobspec might look like a YAML specification for a pod or batch/v1 job, and on a traditional HPC system it might look like a bash script that runs an executable with directives for resources and other parameters. Flux has a form definition of a JobSpec that populates a resource graph.

