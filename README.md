# Sliit-MTIT-Assignment-02

1.Web service Implemented projects 
2.Configured ESB Proxy Services And Soap UI


Eclipse 2019-12 IDE
wso2esb-4.9.0
SoapUI 5.5.0
Postman
Firefox Web Browser


:    SOAP web service and WSO2 ESB activity 
 
Step 1 
 
First of all we create a Dynamic Web Project called “StudentManagementSOAPService” in Eclipse. 

	New > Dynamic Web Project >project_name “StudentManagementSOAPService” > Dynamic web module version as select 2.4 > select Axis web service > Finish

 
 ![Dynamic Web Project](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/1.png)

 ![project_name "StudentManagementSOAPService"](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/2.PNG)
  ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/3.PNG)
 
• Then Implement the Student class and other related class.



Student Class 	
	
	Right click on the project > New > Class > Give the name as “Student” > Finish
   
   ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/4.PNG) 
 
 
 
StudentServiceImple Implementation Class 

	Right click on the project > New > Class > Give the name as “Student” > Finish

  ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/5.PNG) 


 
Step 2 

Create a Web Service application. 

	Right click on the Project > New > Other > Web Service > Service implementation > Browse the StudentServiceImpl > Go to the configuration > Select Server Runtime > Select Apache Axis2 > Ok > Click Publish web service > Start Server > Finish 

  ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/6.PNG) 

 



 

 


 

 

 


 


Test the services and see the output. 
Right click on project > Run As > Run On Service > 
 

▪	getAllStudent function.
 
▪	searchById function.
 


▪	insertStudent Function
 
 
▪	deleteById Function
 
	WSDL file is generated in the web service project as below 

 
 
 

 
 
 
 
 
Step 3 
 
	In this step, we find to wsdl file location .
 
 
 
 
	Then open WSO2 ESB folder and go to the bin. 
 
	Then select wso2sever.bat file and run it. 
 
 
 
  
 







	Then copy the URL which shows on cmd and go for that by using a browser. 

 
  
After that the WSO2 home is displayed, then log in by using,

	username as admin
	password also as admin. 


 



	Click Add > Proxy Service then select WSDL Based Proxy.

 

	Then Add to wsdl file on wso2 ESB. We use in here wso2esb-4.9.0 version.

Select on wso2esb-4.9.0 File > repository > samples > resources > proxy > Paste StudentServiceImple.wsdl file

 



	Then fill relevant fields and click Create to create the WSDL Based Proxy.
 
	Then we can see the created service in the list. 


 

	After that, click and open the service. 
 


Then input the values for request field and send for response. (getAllStudents)
 


 

Then input the values for request field and send for response. (insertStudents)

 
 
Then input the values for request field and send for response. (searchByID)

  

 
 
 
SOAP UI activity 
 
	Copy the WSDL File URL of service .


 
 









	Then open SOAP UI and create a project by using above URL. 

 

 
 









	After that send a request and get response. 


 
 
 
  
 
 
 
 
 
 
 
 
 
 
 

 

 
























	 
