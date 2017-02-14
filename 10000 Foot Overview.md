# (Gregory Thompson) 10,000 Foot Overview of AWS Services

Overview of Services Offered:

- Global Infrastructure
	- Region- Geographic Area containing 2 or more availability zones
	- Availability Zone- AWS Datacenter
	- Edge Location- AWS Datacenter for Content Delivery Network (Remote datacenter Netflix can cache content)

- Network and Content Delivery 
	- Virtual Private Cloud (VPC)
		- Virtual Datacenter (your datacenter in the AWS cloud)
	- Route 53
		- AWS DNS Service (Port 53 is DNS / Old Route 66 Reference)
	- Cloud Front
		- Content Delivery Network for Caching (Edge Locations)
	- Direct Connect
		- Setting up a private, physical, direct line to AWS datacenter
			- More bandwidth, reduced network costs

- Compute
	- EC2 ("Elastic Compute Cloud")
		- Virtual machine in cloud 
	- EC2 Container Service
		- Container Services in EC2 (Docker)
	- Elastic Beanstock
		- Automated Code Deployment
			- Upload code, will automatically provision and deploy all underlying infrastructure underneath the 	             code for you.
	- LightSail  
		- Virtual Private Server (VPS)
		- New this year
		- Affordable and easy to launch
	- Lambda 
		- Server less Computing 
		- Upload code, code responds to external events
		- Exponential, on demand scaling / charged per 100ms of use
		- Supports: JavaScript (Node.js), Python, Java, and C#

- Storage
	- S3 (Simple Storage Service)
		- Virtual disk in cloud
		- Object based storage (.jpeg, .txt, etc.)
	- Glacier 
		- Archival Storage "Cold Storage"
		- Slow retrieval speeds (3-5 hours) / extremely low cost (4/10 penny / gig / month)
	- Elastic File System (EFS)
		- Block Based Storage (applications)
	- Storage Gateway 
		- Connect S3 to on premise datacenter

- Databases
	- Relational Database Service (RDS)
		- SQL, Oracle, Aurora, etc.
	- DynamoDB (Non-Relational Database)
		- NoSQL
	- Redshift
		- Data warehousing solution
			- Run queries on database without interrupting database operations (makes copy).
	- Elastic Cache
		- Caching data in the cloud
		- Static content (such as a product that doesn't change on a sales website)

- Migration 
	- Snowball 
		- Briefcase storage for direct terabytes of data transfer to AWS datacenter 
	- DMS 
		- Database Migration Service (Oracle --> Aurora for example; Oracle is not happy about this)
		- Datacenter to AWS or AWS Location to AWS Location
	- Server Migration Service
		- Virtual Machines / specifically VMWare Machines

- Analytics 
	- Athena 
		- Run SQL Queries on S3 (object storage)
	- Elastic Map Reduce (EMR)
		- Process large amount of data
		- Hadoop or Apache Framework
	- Cloud Search / Elastic Search 
		- Search engine for website or application
	- Kinesis
		- Steaming and analyzing data in real time
		- Stock Markets / Social Media
	- Data Pipeline
		- Move data from AWS Service to another (S3 --> DynamoDB)
	- Quick Sight  
		-  Visualizations

- Security and Identity 
	- Identity Access Management (IAM)
		- Users and Permissions for AWS Services
	- Inspector
		- VM Security Reporting
	- Certificate Manager
		- Free SSL Certifications
	- Directory Services
		- Connect Active Directory to AWS 
	- Web Application Firewalls (WAF)
		- Protect against web application attacks such as SQL Injections
	- Artifacts
		- Compliance Documents

- Management Tools
	- Cloud Watch
		- Monitor AWS performance 
	- Cloud Formation
		- Create production templates, infrastructure to code
	- Cloud Trail
		- AWS Auditing
	- OpsWorks
		- Automated Deployments
	- Config
		- Monitor and Alert for AWS environment (Company Policy Compliance)
	- Trusted Advisor
		- Automated Advice
		- Scan environment / Give tips

- Application Services
	- Step Functions
		- Visualizations inside applications
	- Simple Work Flow (SWF)
		- Coordinating automated and human tasks
		- Amazon fulfillment centers use this to ship items
	- API Gateway
		- Door for apps to access background resources
	- AppStream
		- Stream desktop application to user
	- Elastic Transcoder
		- On the fly transcoder for media

- Developer Tools
	- Code Commit
		- AWS GitHub like service
	- Code Build
		- Code compiler 
	- Code Deploy
		- Deploy code to EC2
	- Code Pipeline
		- Code tracking (across multiple platforms)

- Mobile Services 
    - Mobile Hub
    	- Add/Configure mobile app settings
    - Cognito
    	- Users can sign into application using other identification ("log in through Facebook")
    - Device Farm
   		- Testing application on hundreds of real world iOS/Android devices for QA
    - Mobile Analytics
    - PinPoint
    	- "Google Analytics" for mobile applications on AWS
 
 - Business Productivity
 	- WorkDocs
 		- Storing work documents with extra security features
 	- WorkMail
 		- Email service in AWS

- IOT 
	- New Internet of Things platform on AWS

- Desktop / AppStream
	- Workspaces 
		- Desktop as a Service (DaaS)
		- VDI in AWS to on premise thin/zero client
	- Appstream 2.9
		- Stream desktop apps to users

- Artificial Intelligence
	- Alexa
	- Polly 
		- Text to speech 
		- Most advanced in the world
		- 47 voices in 24 languages currently
	- Machine Learning 
		- Input a dataset and their outcomes and will try to predict future outcomes based on pattern        			recognition.
	- Rekognition
		- Imagine Identification 
			- Facial Recognition 

- Messaging
	- Simple Notification Services (SNS)
		- Notifying users via email or text 
		- ex. notifying admin that AWS environment is crashing
	- SQS 
		- Decoupling Applications
	- Simple Email Services (SES)
	
    
### Needed for Solutions Architect Exam
- Global Infrastructure
- Networking / Content Delivery
- Compute
- Storage
- Databases
- Management Tools
- Security and Identity
- Desktop and App Streaming
- Messaging

### Notes
- AWS seems like a great way to get a quick overhead view of what datacenter operations look like. If someone starts working an entry level position at a company datacenter, it may take years before they even reach a position that deals with an overhead view let alone deals with design. 
- Cloud Guru had a test at the end of this section, scored a 90%, feels good man.
