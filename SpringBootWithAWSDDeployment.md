
**what is cloud computing?<br/>
AWS Introduction?<br/>
Launching EC2 Instance(Linux)<br/>
Connecting to EC2 using Putty (to execute linux commands)<br/>
S3 Bucket(Store Unlimited data in the cloud)<br/>
Deploy Spring Boot Application in EC2 Machine**<br/>
**Application Infrastructure:**<br/>
we cannot give code to client directly we need to set up infrastructure.we setup infrastructure to run run our project.

**Example:**
 we developed springboot application.For springboot application execution we require a server.Application wants to communicate with the DataBase. we need to set up data base server. we need to setup application server , web servers, to handle the load we need to setup load balancer.<br/>
**Lot of infrastructure setup is required inorder to run application.**<br/>
 
**Simple Example how the projects will be deployed in real time :**
DataBase server  to perform  persistant operations.<br/>
we are deploying  application to application server (springboot application Rest API'S).<br/>
If application is deployed to single server.the application cannot handle the load.In real time we  take multiple servers to deploy our application ( load balancing concept).<br/>
Multiple servers will be available to run our application Because application may receive huge numbers of request.<br/>
**Application available in all the servers (example 10 servers) is same. I have created a jar file for my springboot application. same jar is running on multiple servers.As code is same configrutation will also be same.All these servers will be connected to a single database server.<br/>**
**Here if user want to use  application use url1 for server1 url2 for server2 no it is not possiable. If application running in 10 servers .Every server will have its own IP and every server has its own URL.<br/>**
 Therefore here we are going to set up one more server which is called **Load Balancer**.<br/>
 All servers which are running the application are connected to load balancer.<br/>
 For end users we are going to give URL of load balancer.End users you the browser and access the application url (Load Balancer URL).<br/>
 when you send request to LBR , LBR will give request to particular server that server will process your request.(load balancer is used for distrubting the load).<br/>
 To reduce the burden on the servers in real time our application is deployed  on multiple servers and  all servers connected to load balancer which is used to distrube  load to multiple servers.<br/>
 while setting up the servers we need to config the servers, network of server adminstrator of server every things must be taken take of particular organization.you need lot of money and time to setup this type of infrastructure to run your application.<br/>
  overall we need too purchase systems<br/>
  purchase servers<br/>
  purchase database license<br/>
  setup Application infrastructure. db admins, server admins, network admins.<br/>
  setup power connection.<br/>
  seperate room & Internet connection.<br/>
  **To over come this problem and cost we use cloud computing:**<br/>
   To provide IT resources over the internet cloud computing came into the market.<br/>
  **Cloud computing is on demand delivery of IT resources( database, servers, load balancer) over the internet with pay as go pricing( pay only for the amount of time we used)**<br/>
  Instead of buying, owing and maintaining physical data centers and servers, you can access technology services such as computing power, storage and databases, on an as-needed basics.
 **Cloud Advantages:**
 1.Data Security<br/>
 2.Scalability<br/>
 3.Reduced Costs<br/>
 4.Mobility<br/>
 5.Disater Recovery<br/>
 If you go for cloud computing  cloud provider provides infrastructure for rent.<br/>
 There are several cloud providers available in the market.They are providing services over internet with pay as you go model.<br/>
 1.AWS(Amazon)<br/>
 2.Azure(Microsoft)<br/>
 3.Google cloud Platform<br/>
 4.salesforce<br/>
**Cloud services are divided into 3 Types**<br/>
 **1. Infrastructure as service (IAAS)**: They provide servers,database,network,power.We setup servers (Configuration ) to run your application.**They just give you resources**.we need to take care of the setup that is required for that.<br/> 
**2. Platform as service (PAAS)**: Just give  Application source code to cloud provider.<br/>
Cloud provider will prepare infrastructure for your Application.<br/>
Example :I will just give springboot project then cloud proivder will take server setup a network set up a load balancer establish the connection.<br/>
 **3. Software as a service (SAAS)**<br/>
 

  
  



