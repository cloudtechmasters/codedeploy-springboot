# Deploy springboot application in Elastic Bean Stack by using code pipeline

# Pre-Requisites
    Springboot Application
    Write build file
    Need to keep server port number as 5000
    Create Sample Application with in Elastic Bean Stack
 # Create Sample Application with in Elastic Bean Stack
   Goto Elastic Bean Stack and Click on Create application
   ![image](https://user-images.githubusercontent.com/58024415/110230760-19581b00-7f39-11eb-8293-9495df1797b3.png)
   
   Create Environment for sample application
   
   ![image](https://user-images.githubusercontent.com/58024415/110230891-26c1d500-7f3a-11eb-877f-9b4ab72bcb14.png)

   Check application deployed or not and check output of sample application
   
   ![image](https://user-images.githubusercontent.com/58024415/110231287-caac8000-7f3c-11eb-94b9-3936f8243821.png)
   
   Click on above link
   
   ![image](https://user-images.githubusercontent.com/58024415/110231295-e9127b80-7f3c-11eb-999b-16780efe53eb.png)
# Create Code Build
  Goto Code Build
  ![image](https://user-images.githubusercontent.com/58024415/110230955-aa7bc180-7f3a-11eb-9877-61cda3283238.png)
  
  Click on Create Build Project
  
  ![image](https://user-images.githubusercontent.com/58024415/110231256-a355b300-7f3c-11eb-98cd-25f4ed904b2d.png)

# Create Code Pipeline
  Goto Code Pipeline
  ![image](https://user-images.githubusercontent.com/58024415/110231324-224aeb80-7f3d-11eb-9764-01f75a46f023.png)
  
  Click on Create Pipeline
  
  ![image](https://user-images.githubusercontent.com/58024415/110231373-75bd3980-7f3d-11eb-9325-b399a8685a08.png)

  Click on Next
  
  ![image](https://user-images.githubusercontent.com/58024415/110231447-c7fe5a80-7f3d-11eb-9bf4-bc76ba293bf9.png)

  Click on Next
  
  ![image](https://user-images.githubusercontent.com/58024415/110231504-1dd30280-7f3e-11eb-921f-4fea3ce49c33.png)

  Click on Next
  
  ![image](https://user-images.githubusercontent.com/58024415/110231527-3d6a2b00-7f3e-11eb-9dcc-7c7609598733.png)
  
  Click on Next and Click on Create Pipeline
  
  ![image](https://user-images.githubusercontent.com/58024415/110231557-6be80600-7f3e-11eb-9d2a-08c632d6f4b8.png)

Note: It will take time to run code pipeline, once done we can see output of our application using elastic bean stack domain name.

 ![image](https://user-images.githubusercontent.com/58024415/110231699-4c9da880-7f3f-11eb-9c40-a8410afe1f2a.png)
