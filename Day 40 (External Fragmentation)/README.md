# External Fragmentation

When used storage is differentiated into smaller lots and is punctuated by assigned memory space, external fragmentation occurs. It is a weak point of many storage allocation methodologies when they cannot effectively schedule memory used by systems. The consequence is that, while unused storage is available, it is essentially inaccessible since it is separately split into fragments that are too limited to meet the software's requirements. The word "external" derives from the fact that the inaccessible space is stored outside the assigned regions.

Consider, for instance, a scenario in which a system assigns three consecutive memory blocks and then relieves the middle block. The memory allocator can use this unused allocation of the storage for future assignments. Fortunately, if the storage to be reserved is more generous in size than this available region, it will not use this component.

In data files, external fragmentation often exists when several files of various sizes are formed, resized, and discarded. If a broken document into several small chunks is removed, the impact is much worse since this retains equally small free space sections.
