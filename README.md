# codedeploy-springboot.

# Pre-Requisites
    Launch Instance with some tag
    Allow 5000 Port in Security Group
    Install codedeploy-agent
# Launch Instance with Tag   
  ![image](https://user-images.githubusercontent.com/58024415/110238397-6ce15d80-7f67-11eb-8252-f66ea1abafb8.png)
# Install codedeploy-agent
    sudo yum install ruby -y
    wget https://aws-codedeploy-us-east-1.s3.amazonaws.com/latest/install
    chmod +x ./install
    sudo ./install auto
# Create IAM Role for communicating S3 service 
  Goto IAM service  --> Role  -->  Create Role 
  
  ![image](https://user-images.githubusercontent.com/58024415/110240495-2ba27b00-7f72-11eb-9991-c35fa87c2b50.png)

  Click on EC2 and click on Next: Permission
  
  ![image](https://user-images.githubusercontent.com/58024415/110240546-8045f600-7f72-11eb-971d-20622a8a186a.png)

  Click on Next: Tags  --> Next: Review
  
  ![image](https://user-images.githubusercontent.com/58024415/110240568-9f448800-7f72-11eb-891f-7659470c4def.png)

  Click on Create Role
# Attach EC2-S3Role to EC2 Instance and Restart CodeDeploy-agent
    service codedeploy-agent restart
# If you face any issues please check logs of CodeDeploy-Agent
    cat /var/log/aws/codedeploy-agent/codedeploy-agent.log
# Create IAM Role for Code Deploy
  Goto IAM service  -->  Roles  --> Click on create Role

  ![image](https://user-images.githubusercontent.com/58024415/110237776-d0698c00-7f63-11eb-9ffc-b258b2c11700.png)

  Click on CodeDeploy
  
  ![image](https://user-images.githubusercontent.com/58024415/110237814-0f97dd00-7f64-11eb-883e-e6a4f10d9773.png)
 
  Click on CodeDeploy under Select you use case, then click on Next: Permissions --> Next: Tags  --> Next: Review
  
  ![image](https://user-images.githubusercontent.com/58024415/110237882-761cfb00-7f64-11eb-9c3e-02fcfbe64541.png)

  Click on Create Role
# Create Code Build for existing code
  Goto Code Build
  
  ![image](https://user-images.githubusercontent.com/58024415/110230955-aa7bc180-7f3a-11eb-9877-61cda3283238.png)
  
  Click on Create Build Project
  
  ![image](https://user-images.githubusercontent.com/58024415/110231256-a355b300-7f3c-11eb-98cd-25f4ed904b2d.png)
# Create Code Deploy
  Goto Code Deploy
  
  ![image](https://user-images.githubusercontent.com/58024415/110238099-9bf6cf80-7f65-11eb-94f3-e7d9f7fec297.png)

  Click on Create Application
  
  ![image](https://user-images.githubusercontent.com/58024415/110238115-b7fa7100-7f65-11eb-9e18-0bf4a1aeb4a2.png)
  
  Click on Create Application
  
  ![image](https://user-images.githubusercontent.com/58024415/110238270-c301d100-7f66-11eb-8ff9-a08e0042f080.png)

  Click on Create deployment group
  
  ![image](https://user-images.githubusercontent.com/58024415/110238632-baaa9580-7f68-11eb-805e-fe92d10e38e0.png)

  Click on Create deployment group
  
# Create Code Pipeline
  Goto Code Pipeline
  
  ![image](https://user-images.githubusercontent.com/58024415/110238703-19700f00-7f69-11eb-90a6-d349ff35f5d7.png)

  Click on Create Pipeline
  
  ![image](https://user-images.githubusercontent.com/58024415/110238746-46bcbd00-7f69-11eb-9de6-a18db092878b.png)

  Click on Next
  
  ![image](https://user-images.githubusercontent.com/58024415/110238785-8683a480-7f69-11eb-9327-52820c7ec436.png)

  Click on Next
  
  ![image](https://user-images.githubusercontent.com/58024415/110239590-ce0c2f80-7f6d-11eb-9084-dde5fd8ff670.png)

  Click on Next
  
  ![image](https://user-images.githubusercontent.com/58024415/110239609-e1b79600-7f6d-11eb-9b0f-67af3e02e378.png)

  Click on Next and then click on Review
  
  ![image](https://user-images.githubusercontent.com/58024415/110239636-fa27b080-7f6d-11eb-9552-98684f61b4ec.png)

  Will take some time to deploy application in ec2-instance. Once done please check output of application by giving IP address
  
  ![image](https://user-images.githubusercontent.com/58024415/110240431-e4b48580-7f71-11eb-9443-badd4f109ce0.png)
