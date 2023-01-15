<img src="./assets/Ceph_logo.png" alt="Ceph logo" style="width: 450px;" align="right">

# Ceph-quickstarts
Ceph  an open-source software-defined storage platform Quickstarts.

## Intro
- Ceph == software-defined storage (SDS)
- Provides unified software-defined solutions for: 
    - block
    - file
    - object
- Distributed storage sys
- Massively scalable
- High performing
- No single point of faulure
- Exabyte and beyond
- Run on general commodity hardware
- Is a true SDS solution
- Supports: blocks, files, and object storage from a single syst. (that's what makes it *Unified Storage* (new def.))
- Focus on: object storage blocks capabilities (making it *future ready* compared to blocks or files focus)
- It manages not files but objects and supports block-and-file-based storage on top of it
- Objects are better for scalling and increased performance by eliminating metadata operations
- Algos are used to dyn compt where the obj should be stored and retrieved from
- No central lookups to keep track of metadata (caused by reads and writes)
- It uses: CRUSH algo
    - Means: Controlled Replication Under Scalable Hashing
    - It computes on demand where the data should be written to or read from
    - This means no more need to have a centralized table for metadata
    - Distributed accross cluster nodes (computing)
    - Infrastructure awarness:
        - Understands the relationships of various components in the infra
        - unique failure zones, disk, node, rack, row, and data center room
        - It will store data and replicate it to avoid data lost knowing these details
- Self-managing
- Self-healing
- 

> CRUSH mapping needs to be in the correct order.

**RAID:**
> Issue with RAID: 
>
> - Rebuilds are painful
> - If other drives in the RAID group fails it becomes a chaotic situation
> - 

## Unified next-generation storage architecture
- Used to mean: providing file and block storage from a single system
- Now: object storage (because of: cloud computing, big data, IoT)
- Conclusion: all storage that are not supporting of object storage are than not *Unified Storage* solutions

## Architectual philosophy
- All component must scale linearly
- There should not be any single point of failure
- The solutions must be software-based, open source, and adaptable
- The Ceph software should run on readily available commodity hardware
- Every component must be self-managing and self-healing wherever possible

> Object storage is the perfect provision for current and future needs for unstructured data storage.

> In Ceph objects are not tied to a physical path, making objects locations idependent.

## Software-defined storage -- SDS
- SDS helps with TCO (Total Cost of Ownership)
- Benefits: 
    - Flexibility
    - Scalability
    - Reliability

## Cloud storage
- Cloud platform support: 
    - OpenStack
    - Apache CloudStack
    - OpenNebula

## Vendor support
- RedHat
- Canonical
- Mirantis
- SUSE
- etc

## 

## Resources
### Books
- [Ceph: Designing and Implementing Scalable Storage Systems: Design, implement, and manage software-defined storage solutions that provide excellent performance Paperback – Jan. 31 2019](https://www.amazon.ca/gp/product/1788295412/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1)
- [Ceph Cookbook - Second Edition: Practical recipes to design, implement, operate, and manage Ceph storage systems Paperback – Nov. 24 2017](https://www.amazon.ca/gp/product/1788391063/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1)
- [Block Trace Analysis and Storage System Optimization: A Practical Approach with MATLAB/Python Tools Paperback – Nov. 19 2018](https://www.amazon.ca/gp/product/148423927X/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1)
