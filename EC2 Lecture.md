# AWS- EC2 Lecture

EC2 101

 * EC2 is AWS's compute service
 	* Provides resizable compute capacity in the cloud
 	* Allows for quick scaling up or down in capacity

 * EC2 Options
 	* On Demand
 	* Reserved
 	* Spot
 	* Dedicated Hosts

 * On Demand
 	* Low cost, flexibility, without upfront costs
 	* Short time / unexpected work loads
 	* Pay per hour at finite rate
 * Reserved
 	* Provides capacity reservation; 1 or 3 year reservations
 	* For applications with steady state needs
 	* Upfront payments
 * Spot
 	* Applications that have flexible start and end times
 	* Bid for extra compute space
 	* Very low compute prices
 	* NOTE: If EC2 terminates instance, you will not be charged for partial hour
 * Dedicated
 	* Useful for regulatory requirements and licensing that doesn't support multi-tenant virtualization
 	* Can be purchased on demand or reserved

 * EC2 Family Types
 	* D2- Dense Storage - ex. File Server
 	* R4- RAM Optimized - ex. Memory intense applications
 	* M4- General Purpose - ex. Application server
 	* C4- Compute optimized - ex. CPU intensive apps
 	* G2- GPU Optimized - ex. Video Encoding / 3D rendering
 	* I2- High Speed Storage - ex. NoSQL, Data Warehousing
 	* F1- Field Programmable Gate Array - ex. Hardware acceleration for code
 	* T2- Low Cost general Purpose - ex. Web Server
 	* P2- General Purpose GPU - ex. Machine Learning / Bitcoin
 	* X1- Memory Optimized - ex. SAP HANA / Apache Spark

Elastic Bean Stock (EBS)

* EBS
	* Virtual disks you attach to EC2 instancing
	* Block based storage
* EBS Types
	* General Purpose SSD
		* 3 IOPS/gig 
	* Provisioned IOPS SSD
		* I/O Intensive
		* Use with more than 10,000 IOPS requirement
		* Up to 20,000 IOPS  
	* Throughput Optimized HDD
		* Big Data / Data warehousing / log processing
		* Cannot be used as boot volume  
	* Cold HDD
		* Low cost storage for infrequent access
		* File server for example
		* Cannot be boot volume
	* Magnetic
		* Bootable / low cost