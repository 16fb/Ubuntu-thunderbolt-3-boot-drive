# Boot From Thunderbolt

More complicated.
Thunderbolt connector -> is not USB
Rufus doesnt work -> thunderbolt =/= USB, Rufus works with USB only.
Thunderbolt shares a PCIe slot -> threated like internal drive, instead of USB
Solution so far
-> install ubuntu from Live USB, but target the samsung X5 drive. [configure own partitions. swap + journaling.]
-> 


# Solution In The End.
Final Solution:
Install from Live USB, Set EFI, EXT4 Journaling, Swap Partition.
Boot.


# PASSWORD
## Secure Boot
* PASS: AIOT1434

## User Credentials
* USER: AIOT
* PASS: AIOT1434

## Computer Info
* Computer Name -> AIOT
* Visible Name -> AIOT-Alienware-sthsthst