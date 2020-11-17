# Dynamic-Partition Technique

Partitions are created to fit the unique needs of the programs. Main memory is initially viewed as one large empty partition. As programs are loaded, space is “carved out,” using only the space needed to accommodate the program and leaving a new, smaller, empty partition, which may be used by another program later. The operating system maintains a table of partition information, but *in dynamic partitions the address information changes as programs come and go.*

**TL;DR** The computer makes slots that are big enough as it goes.