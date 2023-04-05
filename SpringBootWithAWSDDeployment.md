
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



