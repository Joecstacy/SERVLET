# SERVLET

It is a technology provided by sunmicrosystem, written in java codes.
It runs on server and capable of handeling requests and generating dynamic response.
Although it is a simple java class but there is no main method, it means no use of jvm as it runs on server side.

**#INSTALLATION PART**
Software Requirement:
1. install the eclipse or any IDE to your computer. (for full stack development we should install the Enterprise version only)
2. install the Tomcatserver to your computer.
3. config the Tomcat Server into your IDE.8
    - Open the ecllipse Ide and click on 
    - Windows---->Preferene--->Server---->Runtime Environments
    - Add--->Select the installed Tomcat version--->give the Tomcat directory path---> Finish
4._ Start the Server._
    - Right click on the link avalable bellow
    - New--->Server--->Tomacat installed version--->Next--->Select the current App which u wana deploy
    - Add--->Finish
    - After doing it again right click on the link given bellow--->Start.

**#RULES FOR WRITTING A SERVLET CLASS**
we are having 3 types of servlet API
1. Servlet : It is an interface.
2. GenericServlet: It is an abstract class.
3. HttpServlet: Its an abstract class.

click the link bellow to see the mechanism of the servlet.
![serv1](https://user-images.githubusercontent.com/88554781/162566890-c53856bb-655b-42e3-be68-e9eef8d0661b.jpg)

**#we are having three important methods which we should have to implement.** 
**Servlet Life Cycle**
1. init() : used to initialise the Servlet class. Servlet container initializes the intantiated Servlet object. The container initializes the Servlet object by invoking the Servlet.init(ServletConfig) method which accepts ServletConfig object reference as parameter. The Servlet container invokes the Servlet.init(ServletConfig) method only once, immediately after the Servlet.init(ServletConfig) object is instantiated successfully. This method is used to initialize the resources, such as JDBC datasource.

Now, if the Servlet fails to initialize, then it informs the Servlet container by throwing the ServletException or UnavailableException.
2. service() : It creates the ServletRequest and ServletResponse objects. This method is used to provide the service to the servlet.
3. destroy() : All the resources which we used inside our programe is being done then we will destroy all the resources.

**WRITE YOUR FIRST SERVLET PROGRAM**
1. New--->Dynamic Web Project--->Project name--->Next--->Select source folder and output folder--->Next
2. tick Generate Web xml deployment decriptor---> Finish.
3. FOLDER STRUCTURE
    - src folder --> exm.java file
    - webcontent folder---> Html or jsp file
    - Web INF folder---> web.xml file

