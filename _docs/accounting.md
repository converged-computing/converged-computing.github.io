---
layout: docs
title:  "Accounting"
sections:
  - Example
---

Keeping track of resource usage time, usually on the level of a user or group. This information can be stored in a database and used for making future decisions about scheduling or priority. In terms of units of resource usage, this can vary. 

## Example

HPC uses core-hours (time spent doing the compute). One core-hour equals one CPU core being used for the duration of one hour of execution time. The time is measured as the jobs elapsed wall-clock time from start to finish. [[ref](https://help.itc.rwth-aachen.de/en/service/rhr4fjjutttf/article/090b27dc31484f3c833957978b039b55/), [ref](https://slurm.schedmd.com/accounting.html)]. Cloud does not have the same need for multi-tenancy as HPC, and so accounting to track resource usage is typically associated with cost. Cloud accounts for resources to bill projects, and charges based on data usage or instance cost.

In Flux, accounting is separate from scheduling (flux-sched) as a design choice to make them swappable (e.g., install a different scheduler) however in many HPC managers they are built together, meaning accounting is part of the scheduler.
