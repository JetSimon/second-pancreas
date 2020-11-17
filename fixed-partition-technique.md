# Fixed-Partition Technique

Main memory is divided into a particular number of partitions. The partitions do not have to be the same size, but their size is fixed when the operating system initially boots. A job is loaded into a partition large enough to hold it. The OS keeps a table of addresses at which each partition begins and the length of the partition.

**TL;DR Assign slots on boot and then put the programs in the slots**