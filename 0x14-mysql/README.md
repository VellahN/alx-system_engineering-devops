RAID Redundancy
Perhaps the most common type of replication is RAID. RAID stands for redundant array of independent disks. This means that in most configurations, disks mirror each other in one way or another.

The most basic redundant RAID implementation is a RAID 1 array. This type of array mirrors one disk on another disk. This means that if one disk fails, the other is still available to serve and write data. This type of array speeds up reads due to the fact that the system can read from either of the data locations.

This example is also a great example of why RAID, and redundant setups in general, are not appropriate backups. If you delete a file, it is gone for good. Every change is applied to both disks immediately.

RAID replication is implemented on a low level, so you will not have control over the RAID implementation on a DigitalOcean VPS.

MySQL is a relational database management system, and is the most popular open-source relational database in the world today. It comes installed with a number of built-in replication features, allowing you to maintain multiple copies of your data.
