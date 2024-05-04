---
layout: docs
title:  "Storage"
sections:
  - Example
---
 
> Synonyms: volumes

Storage is transportation of information (i.e., bits) through time [^1]. It is a means to maintain a state of data. While both cloud and HPC provide underlying nodes for storing data, the extent to which the user is able to access and have awareness of the underlying structure varies. Generally speaking, locations vary in the following attributes:

- Frequency of access (frequent vs. infrequent for an archive)
- Permanency of access (temporal or ephemeral for analyses vs. long term archives)
- Permissions (read, write, read/write)
- Cost of storage and operations/access


## Example

For high performance computing, a shared filesystem is provided, and the shared nature is transparent. This means that users are aware of having ownership over a personal space (typically called "home" or a working space called "scratch") or a group space, and are provided tools to allow them to change how data is shared. For cloud, although data storage might have a similar design, the user is presented with a view of sole ownership of a set of locations for storing data. Associated filesystem or object buckets can vary in permissions, node access, and read/write. High performance computing will almost always have shared, often localized storage (a filesystem that supports multiple users with read-write) and in cloud this is almost an anti-pattern. The default (and easiest) setup is usually just read for a single user, and at most read for multiple. Setting up RWX is challenging. For high performance computing, we are interested in supporting a shared filesystem for several kinds of applications, and one with RWX across nodes for applications to share.

[^1]: Feynman's Lectures in Computation (4.1 p. 95) ""Now this isn't exactly the same situation as with memory - which is like sending a message through time rather than space - but you can see the similarities. We store something in memory and at a later time we read it backout - in the interim the stored "message" is subject to noise."
