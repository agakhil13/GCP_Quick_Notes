- 5 Charactersitics of cloud
  - On Demand Self service
  - Broad Network Access
  - Resource Pooling
  - Rapid Elasticity
  - Measured Service
  
- 4 Deployment Models
  - Public cloud - AWS, GCP, AZ ... 
  - Private cloud - on-premises
  - Hybrid Cloud - Private + Public cloud
  - Multi Cloud -  2 or more public cloud

- IaaS
  - Compute Engine (VM instances). You decide what Operating System and software need to install.
- CaaS
  - Google Kubernetes Engine (GKE). For deploying and managing containers.
- PaaS
  - App Engine - Fully managed, serverless platform. Languages - Go, Java, .NET, Node.js, PHP, Python Ruby.
- FaaS
  - Cloud Functions - Serverless execution environment.No need to provision any infra. Languages - JavaScript, Java, node.js, .NET, Python3, Go.
  - Cloud Run - Full Managed for containerized Applications.

- Storage
  - Cloud Storage - Object storage (Region, Dual Region, Multi Region)
    - Standard - Daily access
    - Nearline - < 1/mnt
    - Coldline - < 1/qtr
    - Archival - < 1/yr
	
  - Filestore - NFS storage NFSv3
  
  - Persistent Disk - Block Storage
      - Standard - Regular storage
      - Solid State - Higher IOPs/ lower latency
	
- Databases
  - SQL
    - Cloud SQL - Fully Managed Database service. PostgreSQL, MySQL and SQL Server. HA across Zones.
    - Cloud Spanner - Support transactions, strong consistency and Synchronous replication. HA across regions and globally.
  - NoSQL
    - Bigtable - Fully Managed NoSQL DB. High throughput, low latency. Cluster resizing without downtime.
    - Datastore - Fast, Fully Managed, serverless, NoSQL Document DB. For mobile, web ,IoT. Multi region replication. ACID transaction.
    - Firestore - Real time db. Optimized for offline use. Cluster resizing without downtime.
    - Memorystore - Fully managed. Used for Redis and Memecached.
	  
- Networking
  - Virtual Private Network (VPC)
  - Firewall Rules: 
	  Govern traffic coming into instances on a network.
  - Routes: 
	  Specify how packets leaving an instance should be directed.
  - Load Balancing:
    - HTTP(s) Load Balancing - Distribute traffic across regions to ensure requests are routed to the closest region, during faliure same can routed to next healty instance in the closest region. Distribute traffic based on content type.
    - Network Load Balancing - Distruibute traffic among server instances in the same region based on IP protocol.  
  - Google Cloud DNS
  - Cloud VPN: 
	  Connect your existing network to your VPC through IPsec connection.
  - Direct Interconnect: 
	  Connect your existing network to your VPC through highly available, low latency, enterprise-grade connection.
  - Direct Peering: 
	  Exchange internet traffic between your business network and Google at one of the Google's broad-reaching edge network location.
  - Career Peering: 
	  connect to google's edge location using service providers.
	  
Resource Hierarchy
  - Service level resources
      Compute Instance VM's
	  Cloud storage buckets
	  Cloud SQL databases
  - Account level resources
	  Organization
	  Projects
	  Folders
	  
Cost Management and Budget
  - Committed Use Discounts (CUD's)
	  1 or 3 year commitment
	  Spend based and resource based commitment type
		Spend-based commitment - Discount for a commitment to spend a minimum amount for a service(hour) in a particular region. Available for Cloud SQL and Google CLoud VMWare Engine. Applies only to CPU and memory usage.
		Resource-based commitment - Discount for a commitment to spend a minimum amount for Compute Engine resources in a particular region. Available for vCPU, Memory, GPU and Local SSD. Can be used across projects using shared discount.
  - Sustained-use Discount
	  Automatic discounts for running compute engine resources a significant portion of the billing month. Applies to vCPU and memory for most Compute engine.

GCP pricing Calculator - Can help you to identify the pricing for resources you planned to use.

Cloud Billing Budgets - Enables you to track your actual Google Cloud spend against your planned spend.

Export Billing - Daily cost detail. Pricing. Store in BigQuery.

IAM - Who (Identity) has what access (role) for which resource.
  - Principle of least privilege - Apply only the minimal access level required for what's needed.
  - Set policies at organization or project level rather than at the resource level.
  - Grant roles for users or group at the folder level rather than at rhe project level.
  - Grant roles to Google groups rather than individual users.

Cloud Identity - Identity as a Service (IDaaS)

VPC
  - Can send and receive traffic with IPv4 addresses.
  - Default CIDR /20, can be extended to /16.
  - All IPs fit within subnet 10.128.0.0/9.
  - Auto mode N/w can convert to Custom mode. Reverse is not possible.
  - Google recommend to use custom mode VPC as they are flexible.
  
Flow Logs - Real-time visibility into network throughput and performance. Useful for real-time security analysis.

Load Balancer
  - HTTP(s)
  - SSL Proxy
  - TCP proxy
  - Network
  - Internal
  
BigQuery - For analysis of large data.

Pub/Sub - Queue for notification.

Composer - Built on Apache Airflow, workflow orchestration service 

Dataflow - Apache beam pipelines for batch and realtime datastream,for ETL. Serverless. Cloud Dataflow is a stream and batch processing service

Dataproc - Run hadoop spark on google cloud. Fully managed instance.

Datalab - Tool for machine learning and visualization.

Cloud Data Fusion - Cloud Data Fusion is a managed service that is designed for building data transformation pipelines.

Dataprep - Serverless. Cloud Dataprep is used to prepare data for analytics and machine learning.

Sight - Vision (clasify images and hand written text data). Video Intelligence (recognize a vast number of objecta and streaming videos).

Language - Natural Language (uses unstructred text). Translation (Enables you to translate between languages).

Conversation - Dialog Flow, Speech to text, text to speech.

Auto ML - Fully managed service to build ML product with less knowledge.

Operation Suite (Stackdriver) - Tool for logging, monitoring and application diagnostics. Can also get connect to AWS.

	Monitoring - Cloud Monitoring is used for collecting and view metrics on resource performance.

	Logging - who did what,where and when. Connection records can be viewed in Cloud Logging.

	Error Reporting - Alerts you when new application error occurs.

	Debugger - Cloud Debugger is used by developers to identify and correct errors in code.
	
	Trace - Cloud Trace is used to understand performance in distributed systems.
	
	Profiler - Gather CPU and memory usage from your application.
