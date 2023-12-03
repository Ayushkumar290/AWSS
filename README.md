#  INTRODUCTION TO CLOUD COMPUTING(AWS)  

**What is cloud Computing ?**     
  * The cloud computing is to offers faster innovation, flexible resources, and economies of scale    
  * The cloud computing is to deliverd various cloud sevices like Networking, Scaling, Storage, Databases, Softwere and analytices & Intaligence  

**Benefits of Cloud Computing**  
  * Cost Saving  
  * Loss Prevension  
  * Increased Collaboration  
  * Centralized DATA Security  
  * Scalability  
  * Quality Control  
![cloud-computing-benefits](https://github.com/Ayushkumar290/AWSS/assets/143092664/07eb884b-b630-464e-bef2-6c23019bc5bf)

**Disadvantages of cloud computing**  
  * Downtime  
     * When there is an internet outage or weak connectivity, services get interrupted and this increases downtime.   
  * Security and Privacy  
     * Cloud security measures lead to data leakage over cloud networks which can result in intellectual property theft, contract breaches, and malware attacks.  
  * Vulnerability to Attacks  
     * As these clouds provide services to multiple users over the same network, businesses become vulnerable to cyber attacks which can lead to data loss or data leakage.   
  * Vendor Lock-in  
     * A situation where companies using cloud computing services of a particular vendor are unable to switch to a different vendor.  
  * Cost Concerns  
     * It can also increase expenditure for companies as there are several hidden costs involved which emerge at a later stage. These include data transfer, cloud utilization, and data migration costs.
   
**TYPES OF CLOUD**  
 * PRIVATE
    * Private clouds are distributed systems that work on private infrastructure and provide the users with dynamic provisioning of computing resources.  
 * PUBLICE
    * Public clouds are managed by third parties which provide cloud services over the internet to the public, these services are available as pay-as-you-go billing models.   
 * HYBRID
    * A hybrid cloud is a heterogeneous distributed system formed by combining facilities of the public cloud and private cloud.  

# PRIVATE VS PUBLICE VS HYBRID
![images](https://github.com/Ayushkumar290/AWSS/assets/143092664/9bd5f68d-28af-4be8-8d25-41a632a60b5e)


# AWS`*(Amazon web Service)*  
 * The world's most comprehensive and broadly adopted cloud that includes infrastructure as a service (IaaS) and platform as a service (PaaS) offerings

# COMPUTE SERVICES 
 * EC2 
 * ECS/EKS : containerized services ` 
            * Fargate 
 * lambda : serverless
# Storage Services
 * S3
 * EBS : Amazon Elastic Block Storage is a storage service wherein each block of storage acts like a separate hard drive (volume) . 
 * EFS : dont need to assign any volume , can do on its own , seamless storage , database on EC2 instances
 * Archival service - Glacier : Amazon Glacier is extremely low cost, secure, and durable storage service for data archiving and backup. That data stored which are not needed instantly , eg old data . Takes time min 4 hours or 1 day to retrieve request ( S3 instantly  
   returns request) 
# Network Services 
 * VPC : own insolated environment in a public cloud
 * Domain Name Service - Route 53

# VPC 
 * A secure, isolated private cloud hosted within a public cloud.
![images](https://cf-assets.www.cloudflare.com/slt3lc6tev37/4Tn2beFlmE1Xa8nt6ddphE/c6e9e80aaa3e975dcc798b8e0329949a/virtual-private-cloud.svg)
 **Subnets**: A subnet is a range of IP addresses
 **VLAN**: A LAN is a local area network, or a group of computing devices that are all connected to each other without the use of the Internet
 **VPN**: A virtual private network (VPN) uses encryption to create a private network over the top of a public network.
**SOME VPC PROVIDES ADDITIONAL CUSTAMIZATION**
 **Network Address Translation (NAT)**: This feature matches private IP addresses to a public IP address for connections with the public Internet. With NAT, a public-facing website or application could run in a VPC.
 **BGP route configuration**: Some providers allow customers to customize BGP routing tables for connecting their VPC with their other infrastructure.

# ROUTE 53 
![how-route-53-routes-traffic 8d313c7da075c3c7303aaef32e89b5d0b7885e7c](https://github.com/Ayushkumar290/AWSS/assets/143092664/512cf7b1-4ce0-4894-a49a-56e855c1eb02)

 **DNS** - Domain Name System, translates human readable domain names (for example, www.amazon.com) to machine readable IP addresses (for example, 192.0.2.44). 
# Creating an EC2 Instance 
Step: 1  
![image](https://github.com/Ayushkumar290/AWSS/assets/143092664/811b39cd-ad27-4e17-99e9-002e90567eec)
step: 2 
create a KEY PAIR to access your instamce
step: 3 
Choose your instance type  
step: 4
  Launch instance
 ![image](https://github.com/Ayushkumar290/AWSS/assets/143092664/23c8188b-cea3-4944-bb93-d40bd509d555)
STEP:5 Acces your instance from putty
![image](https://github.com/Ayushkumar290/AWSS/assets/143092664/99e0752a-dcf0-4424-8cbc-a74dfc6821ce)

# Instaling nginx 
for Ubuntu
 ~~~
  $ sudo apt update && apt upgrade
  $ sudo apt install nginx
~~~
for Linux
~~~
  $ yum install nginx
  $ service nginx start
~~~
 **OUTPUT**
![image](https://github.com/Ayushkumar290/AWSS/assets/143092664/dbec75a3-1745-4001-bb52-ecf8dbb1817f) 

# Load Balancing   
 In AWS The sevice called ELB  
* Load Blancing helps in destribution of treffic to other instances to manage load 

* Target Groups - Target groups route requests to individual registered targets 

# crating target groups 
 step: 1  
 ![image](https://github.com/Ayushkumar290/AWSS/assets/143092664/c8c40358-8f53-48d1-aaea-f75f7fb83beb)
 step: 2  
 
