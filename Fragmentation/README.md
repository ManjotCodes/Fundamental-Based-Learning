# What is Fragmentation?

"Fragmentation is a process of data storage in which memory space is used inadequately, decreasing ability or efficiency and sometimes both." The precise implications of fragmentation depend on the specific storage space allocation scheme in operation and the particular fragmentation type. In certain instances, fragmentation contributes to "unused" storage capacity, and the concept also applies to the unusable space generated in that situation. The memory used to preserve the data set (- for example file format) is similar for other systems (- for example, the FAT file system), regardless of the amount of fragmentation (from null to the extreme).

There are three distinct fragmentation kinds: internal fragmentation, external fragmentation, and data fragmentation that can exist beside or a combination. In preference for enhancements, inefficiency, or usability, fragmentation is often acknowledged. For other tools, such as processors, similar things happen.

### The Fundamental concept of Fragmentation

When a computer program demands fragments of storage from the operating system (OS), the elements are assigned in chunks. When a chunk of the software program is completed, it can be released back to the system, making it ready to be transferred to the next or the similar program again afterward. Software differs in the size and duration of time a chunk is kept by it. A computer program can demand and release several blocks of storage throughout its lifetime.

The unused memory sections are large and continuous when a system is initiated. The large continuous sectors become fragmented into a smaller part of the regions through time and utilization. Ultimately, accessing large contiguous blocks of storage can become difficult for the system.


### Internal Fragmentation

Most memory space is often reserved than is required to adhere to the restrictions regulating storage space. For instance, memory can only be supplied in blocks (multiple of 4) to systems, and as an outcome, if a program demands maybe 29 bytes, it will get a coalition of 32 bytes. The surplus storage goes to waste when this occurs. The useless space is found inside an assigned area in this case. This structure, called fixed segments, struggles from excessive memory-any process consumes an enormous chunk, no matter how insignificant. Internal fragmentation is what this garbage is termed. Unlike many other forms of fragmentation, it is impossible to restore inner fragmentation, typically, the only way to eliminate it is with a new design.

For instance, in dynamic storage allocation, storage reservoirs reduce internal fragmentation significantly by extending the space overhead over a more significant number of elements.


The figure mentioned above demonstrates internal fragmentation because internal fragmentation is considered the distinction between the assigned storage space and the needed space or memory.
