# AWS- S3 Labs (pt 1)

Lab 1:
Creating a Bucket

 * Log into AWS --> Go to S3 --> Click on create bucket
 * Bucket names are global and must be globally unique. 
 * No uppercase letters
 * Buckets have various attribute tabs to modify
 	* Versioning
 	* Static Website Hosting
 	* Logging
 	* Tagging
 	* Cross Region Replication
 	* Events
 	* Lifecycle Mangement
 	* Permissions  

Lab 2:
Versioning

 * Go to Bucket's versioning tab --> turn on
 * Can not remove versioning, can only disable
 * Shows files as a single file, however the size is combined depending on how many versions there are

Lab 3:
Cross Region Replication

 * Turn on in Bucket attributes tab
 * Will not copy current objects in bucket unless the object is updated
 * Deleting an object only puts a "delete marker" on it, it doesn't truly delete it.
 * Versioning must be enabled on both buckets.
 * Must be unique regions (can not replicate to same region)
 * Can not replicate multiple buckets (yet)
 * Deleting individual versions or delete markers are not replicated.

Lab 4:
Life Cycle Management

 * Go to Bucket attributes tab --> Turn on lifecycle management
 * Create lifecycle rules for bucket
 	* Move from S3 to IA in X days
 	* Move from IA to Glacier in X days

CloudFront Lecture

 * Content Delivery Network (CDN)
 * Terminology
 	* Edge Location- location where content will be cached
 	* Origin- Origin of CDN file
 	* Distribution- Total CDN Network
 * Two types of CDNs
	* Web Distribution- Typically used for Websites
 	* RTMP- Used for media streaming
 * Objects cached for a set TTL 

Lab 5:
Create a CloudFront CDN

 * Go to CloudFront in AWS
 * Click on Create a CDN
 * Takes usually 20-30 minutes
