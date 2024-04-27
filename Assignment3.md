# Assignment - 3
## Deploy Web application on AWS Cloud (or any cloud)(PHP/Python/Node js any application)

>Name: Aman Narnaware
>
>Roll: 322005
>
>Batch: B1
>
>PRN: 22110404

### 1) Cloud Computing Definition
Cloud computing refers to the delivery of computing services—including servers, storage, databases, networking, software, and more—over the internet ("the cloud") to offer faster innovation, flexible resources, and economies of scale. Essentially, it enables users to access and utilize computing resources on-demand, without the need for direct management of physical infrastructure.

### 2) Cloud Service models and Deployment models
**Service models:**
-  *Infrastructure as a Service (IaaS):* In this model, the cloud provider offers virtualized computing resources over the internet. Users can rent virtual machines, storage, and networking resources on a pay-as-you-go basis. Examples include Amazon Web Services (AWS) EC2, Microsoft Azure Virtual Machines, and Google Compute Engine.

-  *Platform as a Service (PaaS):* PaaS provides a platform allowing customers to develop, run, and manage applications without dealing with the underlying infrastructure. It typically includes development tools, databases, middleware, and other resources. Examples include Google App Engine, Heroku, and Microsoft Azure App Service.

-  *Software as a Service (SaaS):* SaaS delivers software applications over the internet on a subscription basis. Users can access these applications via a web browser without needing to install or maintain any software locally. Examples include Google Workspace (formerly G Suite), Microsoft Office 365, Salesforce, and Dropbox.

**Deployment Models:**
-  *Public Cloud:* Public cloud services are provided by third-party cloud service providers over the internet. These services are available to anyone who wants to use or purchase them. Public clouds offer scalability, cost-effectiveness, and a pay-as-you-go model. Examples include AWS, Microsoft Azure, and Google Cloud Platform.

-  *Private Cloud:* A private cloud is a cloud environment dedicated solely to one organization. It can be physically located on-premises or hosted by a third-party service provider. Private clouds offer enhanced security, control, and customization options, making them suitable for organizations with specific compliance or regulatory requirements.

-  *Hybrid Cloud:* A hybrid cloud combines public and private cloud environments, allowing data and applications to be shared between them. It provides flexibility and allows organizations to utilize the scalability and cost-effectiveness of the public cloud while retaining sensitive data or critical workloads in a private cloud. Hybrid clouds require robust integration and management solutions to ensure seamless operation.

-  *Multi-Cloud:* Multi-cloud refers to the use of multiple cloud computing services from different providers. It involves distributing workloads across multiple clouds to avoid vendor lock-in, improve redundancy, and optimize performance and cost. Multi-cloud strategies often include a combination of public, private, and hybrid clouds, depending on the organization's requirements and preferences.

### 3) Step-by-step screenshot to upload web application on the cloud 
-  Log into your Amazon AWS account.

-  Launch an EC2 instance with HTTP traffic enabled in the security group.
   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/db716ba7-5694-41eb-9872-af27d70a3453)

-  We are creating an simple node app and run it on nginx server.
   Lets install node and npm on this EC2 instance.
   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/23a1ea88-4614-4ac2-bd1d-936f7806db9d)

-  Copy all the website files to the instance. You can use scp for this.
```
scp -i "assignment3.pem" -r website/ ec2-user@ec2-3-108-184-9.ap-south-1.compute.amazonaws.com:/home/ec2-user/website
```
   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/3c953adc-a181-4fa8-9ff0-17b5689ad9c8)

-  Install nginx server on the instace.
```
sudo yum install nginx
```

-  Add the nginx config.
```
server {
    listen 80;
    server_name thisismyassgn3nodeapp.com;

    location / {
        proxy_pass http://localhost:3000;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
    }
}

```

-  Run the node application.

-  Open web browser and search for http://{ip_address}
   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/05287d15-e42c-44e1-81be-fffd590d84c4)

-  Congratulations! you just hosted a website on AWS cloud using nginx server !!
