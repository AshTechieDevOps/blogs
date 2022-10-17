## Gain a Global Reach by Taking the Azure ExpressRoute

Written By Ashish Sharma | Oct 17, 2022
Categories: Azure Cloud, Azure Cloud Networking, Azure Express Route

What is ExpressRoute Global Reach? How does it work and how does it compare with other connectivity options like VNet Peering and Cross-Connections? Why would I need Global Reach? Let's answer all of these questions and more.


-   Global Reach is the product name Microsoft gave to an ExpressRoute service launched in 2018

-   It's basically connecting ExpressRoute connections together so you can send traffic over the Microsoft network rather than all the way into your Azure Virtual Networks and manually manipulating the traffic.

## Here's a simple example scenario where we're using several types of connections so you can see the relationship and use cases for each connection.

![ExpressRoute1](https://user-images.githubusercontent.com/110538923/196165449-d0ca0235-f72e-47bd-b12e-508caa1327ae.PNG)

## Connectivity Between On-Prem and Cloud

-   Very simple ExpressRoute = Connect an on-prem/private network to a virtual network in Azure with ExpressRoute - Pretty vanilla stuff. 'Site A' is connected to 'Azure A' and 'Site B' is connected to 'Azure B' (This could be your private data centre in London connecting to the Azure Europe South data centre for example).

## Connectivity Between Cloud and Cloud

-   VNet Peering = You have resources deployed in a couple of Azure regions, Peering creates a path between your virtual networks in these regions using the Microsoft backbone network. It's a bit like layer 2 invisible VLAN tagging and routing of the traffic to allow BGP both ways. 'Azure A' and 'Azure B' VNets can communicate.

## Connectivity Between On-Prem and Clouds

-   You can add multiple 'Connections' to your ExpressRoute links. In the image above, we have the default connection, from on-prem to cloud (ER Connection 1). A second connection (ER Connection 2) has been added from on prem to the other Azure region. This is sometimes called a 'Cross-Connect' and would allow 'Site A' to talk to 'Azure B' for example.

-   If you didn't have the second connection added to the ExpressRoute, the VNet peering would allow you to make the additional hop from the 'Azure A' VNet to the 'Azure B' VNet from 'Site A'.

## Connectivity Between On-Prem and On-Prem

-   You can use Microsoft's backbone network to communicate between your on-prem sites if they each have an ExpressRoute circuit. This is what we call 'Global Reach'. With Global Reach enabled on 'ER A' and 'ER B', 'Site A' and 'Site B' can communicate directly rather than traversing the Azure virtual networks.

-   This could be used to replace or compliment site-to-site connectivity or enable site-to-site connectivity where it isn't currently present. Yes, you could use a UDR (User Defined Route) to achieve something similar, but this is poor practice and prone to configuration issues and complexity.

Global Reach is basically peering your ExpressRoute's a bit like VNet peering. You can use it in a way that it creates an MPLS-style mesh between your globally distributed sites and various ExpressRoute links, all via the Microsoft Backbone.

![ExpressRoute2](https://user-images.githubusercontent.com/110538923/196166379-fe465363-d993-4524-908e-e381ff73df96.PNG)

## Important Notes

-   Global Reach is not available in all regions, check if your Azure Regions support the service via the link below.

-   VNet to VNet Peering is another way to achieve comms between VNets, it's nothing to do with Global Reach or ExpressRoute for that matter. I just wanted to illustrate the different options.

-   The Route Table on the ExpressRoute Circuit object/resource in Azure will show the advertised ranges, weights and route preferences for those paths that will have multiple routes to the same destination.

-   I've assumed Private Peering on the ExpressRoute circuits. Remember there are two ER Peering types, Private and Microsoft (used to be called Public). Private is a private network to an Azure network. Microsoft Peering is aimed at access to Microsoft services, for example SQL PaaS over ER but this is less common.

## Quick Refresh

For a quick re-cap to jog your memory on some of the technologies that make this all possible;

-   Dot1Q (VLAN) - Industry standard ID via C-Tag (Customer Tag) on the packets, limited to around 4K customers because of the 1-4096 range.

-   QinQ - Layer 2 and used by ExpressRoute, tagging concept is the same as Dot1Q but there's a second encapsulation layer, allowing carriers that provide the transit network to go far beyond the 4K limitation.

-   BGP (Border Gateway Protocol) - Layer 3 - ExpressRoute requires advertising and discovery of network ranges via BGP and where to route to find a specific network range from one AS (Autonomous System) to another. ER uses the ASN (AS-Number) to locate ranges, for example it learns that 10.0.0.4/16 can be found on your private 'Site A' ASN97.

-   VRF - Plays a big part in making all this magic a reality - Virtual Routing and Forwarding. This is basically VLANS for routing at layer 3. Here's an example of a router using VRF versus one without VRF.

![ExpressRoute3](https://user-images.githubusercontent.com/110538923/196167164-8053bc32-f891-4591-8d9b-110795f46c3a.PNG)

## Links for Further Reading

[Azure ExpressRoute](https://learn.microsoft.com/en-us/azure/expressroute/expressroute-global-reach) / [ExpressRoute Global Reach: Building your own cloud-based global backbone](https://azure.microsoft.com/en-in/blog/expressroute-global-reach-building-your-own-cloud-based-global-backbone/)

## About the Author

![ashtechiefinallogo](https://user-images.githubusercontent.com/110538923/196060242-9076fe6b-a236-43b9-bdf7-0d5f1e0b5a8d.png)

I`m Ashish Sharma who brings 24+ Years of Mix & Match Experience of Designing and Architecting Wintel, VMware DCV/NSX/vRO/vRA/vRops, Azure Cloud, Microsoft Cybersecurity, Azure DevOps, AWS, and Google Cloud Solutions offerings.

I am an Expert of Infrastructure as Code using Terraform, Code as Infrastructure (Reverse Terraforming), ARM, Azure Bicep, JSON, AWS CloudFormation, Automation using GitHub Actions, YAML, Jenkins, PowerShell, Azure PowerShell, Configuration Management using Ansible etc. I have very good understanding of Microservices, Containerization aka Open-Source Kubernetes, Docker, Tanzu Grid Cluster and have good knowledge of Scrum, Kanban and other Agile and Project Management tools and methodologies like Microsoft Projects & Jira etc. I am currently exploring “Artificial Intelligence for IT Operations (AIOps)”, specifically Moogsoft.

I do have sound knowledge of Cisco InterSight along with Cisco UCS, Hyperflex, Dell EMC VXRail and other Hyperconverged, Converged & Bare Metal Server Hardware. I have major expertise in Solution Designing of Datacenter and Network Virtualization using VMware vSphere, On-Premises to On-Premises and On-Premises to Cloud Migration & Transformation, Automated & Scripted Migration. I have also taken care of a variety of Greenfield and Brownfield Infrastructure Design, Management, and Security Compliance requirements.

### Contact me

 **⌨️**  [GitHub](https://github.com/ashtechiedevops/) / [LinkedIn](https://www.linkedin.com/in/ashish-sharma-51b3a19/) / [Website](https://ashtechie.com/) / [Twitter](https://twitter.com/ashtechie777/) / [Instagram](https://www.instagram.com/ashtechieworld/)
 
