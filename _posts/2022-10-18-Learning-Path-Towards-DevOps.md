## Learning Path Towards DevOps

Written By Ashish Sharma | Oct 17, 2022

Categories: DevOps, DevOps Learning Path.

![DevOps3](https://user-images.githubusercontent.com/110538923/196544552-28170757-de69-47c2-9d1c-08dda0d48bfc.png)


## This blog is for those who really want to learn Devops, my advice in a few key areas they can focus on.


## Learn a Programming Language:-


-   If you’re like me, with no programming experience, you may be overwhelmed by the sheer amount of programming languages that are out there. For DevOps, my advice would be to pick one of these languages: Python, NodeJS, or Ruby. While it’s important to have a fundamental understanding of all three, you’ll need to be comfortable with at least one in order to progress your understanding of DevOps. 

-   While there is no right or wrong choice when choosing a language, Python is easily the most popular. My recommendation to anyone just beginning to dip their toe into the ocean of programming is to first find a few good videos or written resources that you’ll be able to reference. Afterwards, jump right in. From my experience, the best way to learn programming is to get hands-on and start creating.


## Know Linux Basics:-


-   When it comes to Linux, the guidance remains much the same as with programming. Get into it, get hands-on, and if possible convert your everyday system to Linux. In order to properly grasp the fundamentals, you’ll need to use it daily and in practice. Some key areas you’ll want to focus on are shell commands, Linux directory structure, and SSH key management. 

-   It can be challenging to use “legacy” technology when the operating systems we’re accustomed to using have become so advanced; however, a foundational understanding of Linux is essential for someone learning DevOps. Once you’re comfortable with Linux, you’ll be much more prepared for what’s to come.


## Understand Networking:-


-   Much like the Linux basics, this is another foundational bit of knowledge you just need to know before jumping into the shiny stuff. Networking is the cornerstone of DevOps and the link that enables communications between our applications and users. You’ll need to have a basic understanding of several networking fundamentals: DNS, subnetting, gateways, DHCP, NAT, OSI Model, firewalls, load balancers, proxy servers, and HTTP/HTTPS etc.

## Stick to One Cloud Provider but choice is always yours:-


-   Since we’ve covered the basics, we can start looking at the nice shiny tools that are a keys of DevOps, such as cloud providers. To gain more than just a
    foundational knowledge, you’ll want to pick one cloud provider to concentrate on and stick to it, (The skills you learn here will make your transition much
    easier when exploring other provider options).
     
-   A personal example of mine is that a few years back I began learning AWS, which offers an endless amount of cloud services. I focused on the most common services
    such as IaaS and PaaS, then took those skills with me into Microsoft Azure and Google Cloud Platform. The great thing here is that each of the big cloud providers
    offer a free tier, which enables you to get your hands dirty and gain the experience without financially committing to one provider.


## Use Git Effectively:-


-   Source control is the single most important aspect of DevOps. Understanding Git and being able to use it effectively is essential to your workflow.

-   Every script you create should be managed through source control, so that you can track changes and collaborate with other developers. You’ll need to understand
    the concepts of branching, pull requests, and code repositories, as well as how they fit into the overall development process.

-   GitHub is easy and the most popular code repository platform, and where I personally store much of what I’ve learned to GitHub only. 

## Containers? Start with Docker:-


-   When you think of containers, you think of Docker, and this is where I’d recommend you should start your container learning.

-   Containers allow for a consistent and portable environment for applications to run on. When it comes to learning Docker, make sure to get hands-on experience. This is super easy to do as pretty much anything can run Docker. 

-   You’ll want to be able to create, run, download, change, and inspect containers. It’s also important that you understand the networking stack, storage management, and the creation of your own Dockerfiles.


## Orchestrate with Kubernetes:-


-   Now that we’re comfortable with containers, we’ll need to understand how to orchestrate them. Kubernetes is a container orchestration engine that allows you to manage a large amount of containers over multiple nodes. There are a variety of resources out there that will help you learn about Kubernetes in-depth, both in theory and hands-on. 


## Learn Infrastructure as Code:-


-   Code is not just about applications. You should also be learning about how we use code to create your infrastructure. This could be in the public cloud, on premises in your virtualization environments, or in your home lab. Infrastructure as code (IaC) is the way to build infrastructure in a safe and repeatable way.

-   Terraform is a great tool for learning infrastructure as code. Terraform allows for you to write, plan, and apply desired state changes to your infrastructure for multiple providers. Terraform understands the current state of your deployment and retains it for you.

-   This lends itself nicely to repeatability. We’ve all been there: you find yourself needing to deploy virtual machines multiple times in different locations. Terraform and other IaC tools easily make this for you. 


## Automate Configuration Management:-


-   Our next step towards DevOps automation is to ensure that the desired state of our deployed applications is retained. While IaC enables you to build a platform in a repeatable way, configuration management will provide similar benefits on the application side of things. Tools such as Ansible, Puppet, Chef and Salt  provide a simple way to automate your configuration management.

## Learn, Understand and Create CI/CD Pipelines:-


  So we know how to maintain the state of our application, but how do we actually get it to that desired state? Time to automate the process of creating applications.
 
  There are two aspects to consider when creating your pipeline: Continuous Integration and Continuous Deployment (CI/CD):-
  
  
-   Continuous Integration: If you have been scratching the surface of DevOps, you’ll have most likely come across the terms Code > Build > Test. This process is the foundation of getting application code tested and ready to release to your audience.

-   Continuous Deployment/Delivery: Continuous Deployment/Delivery will enable you to update your application in an automated fashion. If the code passes its tests, use continuous deployment to push that code into the next environment be it, QA, staging, or production.

-   Some commonly used tools for creating CI/CD pipelines are: GitHub Actions, Jenkins, TravisCI, and GitLab etc.


## Monitoring, Log Management, and Data Visualization:-


-   Keep in mind that throughout this journey, many important security and logging techniques are foregone, for the sake of education. Many of the tools discussed here ensure proper configuration with security in mind, but the integrity of your applications is your responsibility. You should make certain that your application is secure before pushing it to production.

-   It’s also important to consider how your systems collect and aggregate data. Finding a way to visualize the information you collect can be extremely useful when analyzing trends and to mitigate risk. Tools such as Prometheus, Grafana, and ELK stack (Elasticsearch, Logstash, and Kibana) should be on your radar while you’re trying to understand this area of DevOps.


## Store and Protect Your Data:-


-   At some point in your journey, you are going to require a level of stateful data, be it some sort of persistent storage for storing logs or an actual database requirement. This is where data management comes in. You’ll need to know where to store the dataset, as well as how to best protect the data.

-   It should be noted that no platform is completely safe from data loss, accidental deletion, or malicious activity. However, by automating most of the workflow, we can eliminate the majority of human error from our development pipeline. At the end of the day, the integrity and management of application data will always fall on the shoulders of DevOps.

-   There are a lot of different database options to explore. I’d advise you to learn the fundamentals of backing up data, managing application mobility between environments, and disaster recovery.
  
  
## I Wish You a Good Luck on Your DevOps Journey!


## About the Author:-

![ashtechiefinallogo](https://user-images.githubusercontent.com/110538923/196060242-9076fe6b-a236-43b9-bdf7-0d5f1e0b5a8d.png)

I`m Ashish Sharma who brings 24+ Years of Mix & Match Experience of Designing and Architecting Wintel, VMware DCV/NSX/vRO/vRA/vRops, Azure Cloud, Microsoft Cybersecurity, Azure DevOps, AWS, and Google Cloud Solutions offerings.

I am an Expert of Infrastructure as Code using Terraform, Code as Infrastructure (Reverse Terraforming), ARM, Azure Bicep, JSON, AWS CloudFormation, Automation using GitHub Actions, YAML, Jenkins, PowerShell, Azure PowerShell, Configuration Management using Ansible etc. I have very good understanding of Microservices, Containerization aka Open-Source Kubernetes, Docker, Tanzu Grid Cluster and have good knowledge of Scrum, Kanban and other Agile and Project Management tools and methodologies like Microsoft Projects & Jira etc. I am currently exploring “Artificial Intelligence for IT Operations (AIOps)”, specifically Moogsoft.

I do have sound knowledge of Cisco InterSight along with Cisco UCS, Hyperflex, Dell EMC VXRail and other Hyperconverged, Converged & Bare Metal Server Hardware. I have major expertise in Solution Designing of Datacenter and Network Virtualization using VMware vSphere, On-Premises to On-Premises and On-Premises to Cloud Migration & Transformation, Automated & Scripted Migration. I have also taken care of a variety of Greenfield and Brownfield Infrastructure Design, Management, and Security Compliance requirements.

### You can connect with me by using any of the below given communication channels:-

 **⌨️**  [GitHub](https://github.com/ashtechiedevops/) / [LinkedIn](https://www.linkedin.com/in/ashish-sharma-51b3a19/) / [Website](https://ashtechie.com/) / [Twitter](https://twitter.com/ashtechie777/) / [Instagram](https://www.instagram.com/ashtechieworld/)
 
