**What is unit testing?<br/>
why Unit testing?<br/>
what is Junit?<br/>
Junit5 Introduction<br/>
Junit5 Architecture<br/>
Unit Testing Examples<br/>
Mocking<br/>
Rest API Unit Testing<br/>
Code  Coverage Using Jacocoo<br/>**
**-----------------------------------------------------------------------------------------------------**<br/>
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
**------------------------------------------------------------------------------------------------------**<br/>
**What is Junit?**
 Unit testing can be performed in 2 ways one is manual unit testing and second is automatic unit testing.
Manual unit testing means you going to that method excetute method and see how method is working or we use debugging (in debugging you can execute the program line by line)
 
Nows a days  we can perform automated unit testing  It saves our time.

**Note: Junit is a free and open source unit Testing framework for  java applications.It is easy to use.**<br/>
**It is a light weight testing framework which allowed java developers to write unit test cases in Java Language.**<br/>
In DAO layer:<br/>
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
}<br/>
**Note:The  current version of Junit is 5**<br/>
**-------------------------------------------------------------------------------------------------------**<br/>
**Implementing Junit:**<br/>
1. add Junit dependency. in scope it is mentioned as  test only when test cases are running these dependency must be added to class path of the application.<br/>
**Junit 5 Architecture**<br/>
3 main modules in the Junit 5.<br/>
**1.Junit Platform.<br/>
2.Junit Jupiter.<br/>
3.Junit Vintage.<br/>**
**1. Junit Platform:** This provide  an environment to run junit test cases using junit5.<br/>
**2.Junit Jupiter:** It provides new annotations & new assertions in Junit5 for better unit testing.<br/>
**3.Junit Vintage:** Provide Backward Compatability ( Junit 3 support, Junit 4 support).<br/>

**----------------------------------------------------------------------------------------------------------**<br/>
**Junit 5 Annotations :** <br/>
1.**@Test** -  used to represnt one method as unit test method.<br/>
2.**@BeforeEach**-  I want to execute some logic before each test method <br/>
3.**@AfterEach**-   I want to execute some logic after each test case.<br/>
4.**@BeforeAll**-   Before all test methods we want to execute one logic.<br/>
5.**@AfterAll**-    After all test methods we want to execute one logic.<br/>
6.**@ParameterizedTest** - multiple inputs for one test method (below 4 are used for parameterized testing).<br/> 
7.**@ValueSource**-  to supply inputs for parameterzied  test.<br/>
8.**@CsvSource**<br/>
9.**@CsvFileSource**<br/>
10.**@MethodSource**<br/>
11.**@RepeatedTest**- repeat test method  for execution for fixed  number  of times.<br/>
12.**@Disabled**-  If we want to stop one test method execution.<br/>
**---------------------------------------------------------------------------------------------------------------**<br/>
**Junit 5 Assertions :**<br/>
Junit 5 assertions help us in validating the expected output with the actual output of a test case.<br/>
In short assertions are nothing but static methods that we  call in our tests to verify the expected behaviour.<br/>
All Junit Jupiter assertions are present in the org.junit.jupiter.Assertions class.<br/>
**Junit Assertion Methods :**<br/>
**1.assertEquals and assertNotEquals<br/>
2.assertTrue and assertFalse<br/>
3.assertNull and assertNotNull<br/>
4.assertSame and assertNotSame<br/>
5.assertThrows**<br/>

















