# Boot From Thunderbolt
More complicated.
Thunderbolt connector -> is not USB
Rufus doesnt work -> thunderbolt =/= USB, Rufus works with USB only.
Thunderbolt shares a PCIe slot -> threated like internal drive, instead of USB
Solution so far
-> install ubuntu from Live USB, but target the samsung X5 drive. [configure own partitions. swap + journaling.]
# Solution In The End.
Final Solution:
Install from Live USB, Set EFI, EXT4 Journaling, Swap Partition.
Boot.

**EFI Partiton**
EFI Space -> 100MB
Type -> Primary
Use as -> EFI Boot Partion

**EXT4 Data Partition**
EXT 4 Partition
Partition Type -> Primary
Space Size -> All remaining space
Use as -> EXT4 Journaling file system.
Location -> start of this space
Mount Point -> /


Size -> Space == RAM present in system.
Type of partition -> Logical
Location -> Beginning of space
Use as -> Swap area