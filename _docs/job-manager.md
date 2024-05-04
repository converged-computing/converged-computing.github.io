---
layout: docs
title:  "Job Manager"
#sections:
#  - Example
---

The job manager receives new jobs, and is in charge of moving them through states. As an example, the Flux Framework job manager defines states new, depend, priority, sched, run, and cleanup. Each state might trigger events or connections to other components of the batch system.
