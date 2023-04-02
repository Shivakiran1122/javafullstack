**Agenda:<br/>
What is unit testing?<br/>
why Unit testing?<br/>
what is Junit?<br/>
Junit5 Introduction<br/>
Junit5 Architecture<br/>
Unit Testing Examples<br/>
Mocking<br/>
Rest API Unit Testing<br/>
Code  Coverage Using Jacocoo<br/>**

**What is Unit testing and why?**<br/>

1.Unit Testing  is type of software testing where individual units or components of a software are tested.<br/>
In Application development we are going to create several classes in the classes we are going to create several methods.we need to test these methods whether they are working as excepted or not.<br/>
2. The purpose is to validate that each unit of the software code performs as excepted.<br/>
suppose you write method in the  controller  controller method calls service layer method. service layer method  calls  DAO method. DAO method interacts with data base here we are following layered architecture  we are following to develop that application.
Once we complete DAO method we first test that DAO method.<br/>
3.Unit testing  is done during the development(Coding phase) of an application by the developers.<br/>
4.Unit Tests isolate a section of code and verify its correctness.<br/>
we have controller method controller talks to service method as part  of unit testing we will only test controller method.<br/>
Note: Unit  may be individual function , method, procedure, module or object.

**In real time project:**
1.first if I write DAO Layer method. We will write unit testing logic for that DAO layer. after Dao layer implementation and testing is completed then we go for service in sevice we do the same thing, then after that in controller same thing. so this way the quality  of the code is been maintained.

**What is Junit?**
 Unit testing can be performed in 2 ways one is manual unit testing and second is automatic unit testing.
Manual unit testing means you going to that method excetute method and see how method is working or we use debugging (in debugging you can execute the program line by line)
 
Nows a days  we can perform automated unit testing  It saves our time.

**Note: Junit is a free and open source unit Testing framework for  java applications.It is easy to use.**<br/>

**It is a light weight testing framework which allowed java developers to write unit test cases in Java Language.**<br/>
In DAO layer:<br/><br/>
public USER findByEmailAndPwd(String email, String pwd)<br/>
{
 // db logic to retrive record<br/>
 if(isPresent)<br/><br/>
{
 return userObj;
}
 return null;<br/>
}


perform unit testing for above method<br/>

public void testfindByEmailAndPwd()<br/>
{
// unit testing logic (using Junit)<br/>
}
**Note:The  current version of Junit is 5**<br/>

**Implementing Junit:**<br/>
1. add Junit dependency. in scope it is mentioned as  test only when test cases are running these dependency must be added to class path of the application.<br/>



