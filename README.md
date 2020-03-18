
[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)



# Sliit-MTIT-Assignment-02 

```sh

1.Web service Implemented projects 
2.Configured ESB Proxy Services And Soap UI

```


```sh

Eclipse 2019-12 IDE
wso2esb-4.9.0
SoapUI 5.5.0
Postman
Firefox Web Browser

```

# SOAP web service and WSO2 ESB activity 
 
### Step 1 
 
First of all we create a Dynamic Web Project called “StudentManagementSOAPService” in Eclipse. 

	New > Dynamic Web Project >project_name “StudentManagementSOAPService” > Dynamic web module version as select 2.4 > select Axis web service > Finish

 
 ![Dynamic Web Project](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/1.png)
 

 ![project_name "StudentManagementSOAPService"](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/2.PNG)
 
 
 ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/3.PNG)
 
 
• Then Implement the Student class and other related class.



### Student Class 	
	
	Right click on the project > New > Class > Give the name as “Student” > Finish
   
   ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/4.PNG) 
 
 
 
### StudentServiceImple Implementation Class 

	Right click on the project > New > Class > Give the name as “StudentServiceImple” > Finish

  ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/5.PNG) 


 
## Step 2 

Create a Web Service application. 

	Right click on the Project > New > Other > Web Service > Service implementation > Browse the StudentServiceImpl > Go to the configuration > Select Server Runtime > Select Apache Axis2 > Ok > Click Publish web service > Start Server > Finish 


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/6.PNG) 



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/7.PNG)



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/8.PNG)



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/9.PNG)



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/10.PNG)



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/11.PNG)



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/12.PNG)



Test the services and see the output. 

	Right click on project > Run As > Run On Service > 
	 

![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/new/111.PNG)



▪	getAllStudent function.


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/new/222.PNG)



▪	searchById function.


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/new/333_search_by_id.PNG)



▪	insertStudent Function


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/new/444_insert_Student.PNG)
  


▪	deleteById Function


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/new/555_delete_by_id.PNG)

 
 
 WSDL file is generated in the web service project as below 


  ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/13.PNG)
  


## Step 3 
 
### In this step, we find to wsdl file location .


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/14.PNG) 
 

### Then open SOAP UI and create a project by using above URL. 


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/15.PNG) 



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/16.PNG)



### After that send a request and get response. 


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/17.PNG) 



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/18-insert(1).PNG) 



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/18-result(2).PNG) 



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/19-findbyid.PNG) 




### In this step, we find to wsdl location using soapUI.
 
 
![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/soapui.PNG)  
 
 
 
* Then open WSO2 ESB folder and go to the bin. 
	
* Then select wso2sever.bat file and run it. 
 
 
![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/TT.PNG) 
 
 
 
### Then copy the URL which shows on cmd and go for that by using a browser. 

 
 ![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/20-stating_WSO2.PNG)
 
  
### After that the WSO2 home is displayed, then log in by using,


```sh

* username as admin
* password also as admin. 

```

![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/21-signin.PNG.PNG)
 


	Click Add > Proxy Service then select WSDL Based Proxy.
	

![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/22-select-wsdl.PNG)


 
### Then Add to wsdl file on wso2 ESB. We use in here wso2esb-4.9.0 version.

	Select on wso2esb-4.9.0 File > repository > samples > resources > proxy > Paste StudentServiceImple.wsdl file


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/Capture.PNG)


 
### Then fill relevant fields and click Create to create the WSDL Based Proxy.


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/23.PNG)



### WSDL Service and WSDL Port Can be finding on our WSDL url


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/oop.PNG)


### Then we can see the created service in the list. 


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/zz.PNG)



### After that, click and open the service.
		
	
	Then input the values for request field and send for response. (getAllStudents)
	


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/111.PNG)



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/222.PNG)




### Then input the values for request field and send for response. (insertStudents)



![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/333.PNG)
 



### Input the values for request field and send for response. (searchByID)


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/444.PNG)




### Input the values for request field and send for response. (deleteByID)


![](https://github.com/Ranushklakmal/Sliit-MTIT-Assignment-02/blob/master/Screenshot/555.PNG)

  


![](https://twemoji.maxcdn.com/36x36/1f3c1.png)
&copy; Ranushka Lakmal ![](https://twemoji.maxcdn.com/36x36/1f3c1.png)

  

	 
