# AWS- S3 Labs (pt 2)

S3 Security and Encryption Lecture

 * New buckets are private
 	* Can change with bucket policies
 * Encryption Types
 	* In Transit
 		* SSL/TLS (HTTPS)
 	* At Rest
 		* Severside
 			* S3 Management Keys (AES-256)
 			* AWS Key Management Service (Audit Trail)
 			* Serverside w/ customer provided keys
 		* Clientside Encryption
 			* Encryption on client then upload to S3
 
 
Storage Gateway Lecture

 * Connects on premise service with AWS Cloud
 * Download as VM Image
 	* Install on hypervisor in datacenter
 * 4 Types
 	* File Gateway (NFS)
 		* Flat files to S3
 	* Volumes Gateway (iSCSI)
 		* Block based storage
 		* 2 Types
 			* Stored Volumes
 			* Cached Volumes
 	* Tape Gateway (VTL)
 		* Backup and archival virtual tape cassette

AWS Snowball

 * Accelerate large data upload speeds to AWS via physical unit
 * Types
 	* Snowball
 		* Briefcase sized
 		* Petabyte scale transfer (80TB units)
 		* 256 bit encryption
 		* Tamper resistant
 	* Snowball Edge
 		* 100TB units
 		* Compute capability
 		* Can run Lambda functions (ex. airplane data collection in flight)
 	* Snowmobile
 		* Petabyte to Exabyte data transfer
 		* Sea container on a semi truck
 		* 100 PB per unit
 		
AWS Transfer Acceleration

 * Cloudfront Edge Network to accelerate uploads to S3

AWS Create a Static Website Lab

 * Create a S3 bucket
 * Enable Static Website Hosting
 * Set file designations
 * Upload HTML files
 * Good to go
