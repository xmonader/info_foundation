## Threefold Cloud Units (TCU)


The ThreeFold Capacity is expressed in units.  These units have the following definitions:

To measure processing power available in the presented Threefold capacity

| CU (Compute Unit) | Type  | A     | B     | C        | .     |
| :---------------: | ----: | :---: | :---: | :------: | :---: |
| GB Memory         | 4     | 8     | 2     |          |       |
| nr vCPU           | 2     | 1     | 4     |          |       |
| Min Frequency     | 1,600 | 800   | 3200  | MHz      |       |
| Max Frequency     | 4,000 | 2,000 | 8000  | MHz      |       |
| Passmark Min      | 500   | 250   | 1000  | Passmark |       |
| Passmark Max      | 1,250 | 625   | 2500  | Passmark |       |


| SU (Storage Unit)               |                     | Archive\[^1\] \(*\) | Nas[^1] | Std Disk[^2] | DB Disk[^2] | Temp Disk | .     |
| ------------------------------- | ------------------: | :-------------: | :-----: | :----------: | :---------: | :-------: | :---: |
| GB Storage Capacity | 1,000           | 400     | 50           | 5           | 80        | GB    |
| burst performance (TPS)         | 20                  | 100             | 10,000  | 40,000       | 10,000      |
| sustained min performance (TPS) | 5	25                | 1,000           | 4,000   | 1,000        |
| redundant                       | Y                   | Y               | Y       | Y            | N           |
| min size                        | 1,000               | 1,000           | 10      | 40           | 10          | GB        |
| max size per vnas or vdisk      | 10,000,000          | 1,000,000       | 500     | 500          | 500         | GB        |

| NU (Network Unit = per GB)                | .     | .     |
| :---------------------------------------: | :---: | :---: |  |
| GB transfered OUT or IN                   | 1     | GB    |
| GB transfered in country/region OUT or IN | 5     | GB    |

\[^1\]:  calculated using policy of 20 backend nodes, 4 of any nodes can be lost at any point in time, blocksize = 1MB

\[^2\]: calculated using replica of 2, so 2 copies of each block/object stored
