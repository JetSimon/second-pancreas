# Paged Memory Management

In the paged memory technique, main memory is divided into small fixed-size blocks of storage called frames. A process is divided into pages that (for the sake of our discussion) we assume are the same size as a frame. 

When a program is to be executed, the pages of the process are loaded into unused frames distributed through memory. Thus the pages of a process may be scattered around, out of order, and mixed among the pages of other processes. 

To keep track of these pages, the operating system maintains a separate page-map table (PMT) for each process in memory; it maps each page to the frame in which it is loaded.

![](https://i.imgur.com/sK43Y6Y.png)

A logical address in a paged memory management system begins as a single integer value relative to the starting point of the program, as it was in a partitioned system. This address is modified into two values, a page number and an offset, by dividing the address by the page size. The page number is the number of times the page size divides the address, and the remainder is the offset. So a logical address of 2566, with a page size of 1024, corre- sponds to the 518th byte of page 2 of the process. A logical address is often written as <page, offset>, such as <2, 518>.

A logical address of <1, 222> would be processed as follows: Page 1 of process 1 is in frame 12; therefore, the corresponding physical address is 12 * 1024 + 222, or 12510. Note that there are two ways in which a logical address could be invalid: The page number could be out of bounds for that process, or the offset could be larger than the size of a frame.

The advantage of paging is that a process no longer needs to be stored contiguously in memory. The ability to divide a process into pieces changes the challenge of loading a process from finding one large chunk of space to finding many small chunks.

An important extension to the idea of paged memory management is the idea of demand paging, which takes advantage of the fact that not all parts of a program actually have to be in memory at the same time. At any given point in time, the CPU is accessing one page of a process. At that point, it doesn’t really matter whether the other pages of that process are even in memory.

In demand paging, the pages are brought into memory on demand. That is, when a page is referenced, we first see whether it is in memory already and, if it is, complete the access. If it is not already in memory, the page is brought in from secondary memory into an available frame, and then the access is completed. The act of bringing in a page from secondary memory, which often causes another page to be written back to secondary memory, is called a page swap.

Excessive page swapping is called thrashing and can seriously degrade system performance.