# Single Contiguous Memory Management

The approach to memory management in which a program
is loaded into one continuous area of memory.

Only one program other than the operating system can be processed at one time. To bind addresses, all we have to take into account is the location of the operating system.

If the program is loaded starting at address A, then **the physical address corresponding to logical address L is A + L.** 

**EXAMPLE:** Program is loaded into memory beginning at address 555555. When a program uses relative address 222222, we know that it is actually referring to address 777777 in physical main memory.