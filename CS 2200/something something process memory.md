Internal fragmentation is space in a partition wasted.
We can deal with this using variable size partitions


External fragmentation is sum of all non-contiguous free memory partitions. If there is only one piece of a memory block there is 0 external fragmentation.

First fit
Best Fit
Next Fit
If we have dynamic fragmentation we can move processes to reduce external fragmentation
We can try making our processes non-contiguous. Can split into fixed size chunks called pages
Broker can be used to 

Address is then made up of virtual page number and offset. We use VPN to index into the page table. Page table goes into physical memory



Locality. Most data we look at is adjacent.
