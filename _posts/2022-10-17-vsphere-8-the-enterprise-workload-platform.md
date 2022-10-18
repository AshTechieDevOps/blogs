## Introducing vSphere 8: The Enterprise Workload Platform
Written By Ashish Sharma | Oct 17, 2022

Categories: VMWare, VMWare vSphere8, VMWare Solution for Datacenter Virtualization, DevOps, VMware Tanzu Kubernetes.

![vSphere8_1](https://user-images.githubusercontent.com/110538923/196090426-f7f6cce2-4dfc-446d-b26f-da6ec90b5dc0.PNG)

## Workloads are growing everywhere

As organizations embrace cloud, they are beginning to turn a new chapter in the era of multi-cloud. Multi-cloud has quickly become the dominant deployment model. According to a 451 Research study, 75% of all enterprises have multi-cloud footprints (1). Many enterprises choose to run mission critical workloads on-premises to take advantage of data locality, predictable workload performance and low network latency. As larger masses of data accumulate in the enterprise, they tend to attract more local services and applications to minimize latency, increase throughput, and maximize workload performance.

![vSphere8_2](https://user-images.githubusercontent.com/110538923/196090935-132ba2e2-23d2-4dfc-8b3b-fe24f9e84f91.PNG)

## Consumption model preferences are evolving

IDC predicts that by 2025, 60% of enterprises will fund projects through OpEx budgets(2). This trend is evident with IT organizations continuing to embrace cloud-based consumption models for infrastructure services. Lines-of-business are increasingly making their own choices for infrastructure and services based on unique needs. Software-as-a-service is quickly emerging as a central strategy that businesses are adopting to save time and achieve goals quicker. In fact, Gartner expects worldwide SaaS spending to reach $208 Billion by year 2023(3).

## Demand for infrastructure services is increasing

The volume and complexity of modern workloads are increasing, which is creating higher demand for infrastructure services that provide key underlying functionality for these workloads. The increasing demand for software defined infrastructure services places more strain on CPUs, leaving fewer compute cycles for workloads. Newer classes of hardware accelerators like Data Processing Units (DPUs, also known as SmartNICs) have been successfully used by hyperscalers to offload and accelerate infrastructure functions, freeing up CPU cycles to run workloads. As DPUs become more mainstream in the infrastructure, there is an increasing number of hardware choices from vendors with varying sets of capabilities. IT infrastructure teams are faced with the challenge of abstracting the hardware differences and presenting a uniform consumption interface to users.

## Security threats to Data Center traffic are rising

Modern applications are also increasingly micro-services based and drive-up East-West network traffic within the data center. When it comes to securing the enterprise network, traditional firewalls focus solely on the network perimeter, with limited understanding of application topologies and behaviors. Traditional distributed firewalling approaches require host-based agents to secure the network within the data center, and result in complex security architectures and operations. With workloads and infrastructure services sharing a domain, the chances of malicious actors penetrating the network perimeter and persisting in the network are higher.

## Traditional approaches to meet the needs of next-gen infrastructure do not work

Adding new server capacity to meet the increasing demand for infrastructure results in higher total cost of ownership. Application specific silos, such as GPU-based servers for running AI/ML workloads, do not scale well to run traditional IT workloads. This results in an inflexible architecture that leads to additional operational complexities. In a converged domain where workloads run alongside infrastructure services, the CPU complex becomes a single point of failure as has been shown by low level security exploits in the recent past.

On top of it all, IT organizations are expected to deliver uniform infrastructure consumption experiences across multi-clouds to develop, deploy and maintain high performant applications in a cost-effective and secure manner.

What if you could supercharge workload performance while scaling infrastructure services across the enterprise and reduce the total cost of infrastructure?

What if you could enable development teams to accelerate their innovation and deliver IaaS services directly to their development environments?

What if the benefits of cloud were made available to on-premises workloads without requiring lift-and-shift?

What if you could centrally manage on-premises infrastructure and reduce the operational burden of maintenance?

Well, the time to wonder ‘what if’ is over.

## Introducing VMware vSphere 8

VMware vSphere 8, the enterprise workload platform, brings the benefits of cloud to on-premises workloads, supercharges performance through DPUs and GPUs, and accelerates innovation with an enterprise-ready integrated Kubernetes runtime. Let’s get into more detail.

![vSphere8_3](https://user-images.githubusercontent.com/110538923/196091608-85034868-2a04-4b72-bd85-b6d7e215a762.PNG)

vSphere 8 ushers in a new era of heterogeneous computing by introducing Data Processing Units to Enterprises through VMware vSphere Distributed Services Engine. vSphere Distributed Services Engine is the next step in the evolution of cloud infrastructure for modern applications, in which the stewardship for running infrastructure services is distributed between the CPU and the DPU.

vSphere Distributed Services Engine modernizes cloud infrastructure into a distributed architecture enabled by DPUs to:

-   Meet the throughput and latency needs of modern distributed workloads by accelerating networking functions.

-   Deliver best infrastructure price-performance by providing more CPU resources to workloads.

-   Reduce operational overhead of DPU lifecycle management with integrated vSphere workflows.

vSphere Distributed Services Engine preserves the existing Day-0, Day-1 and Day-2 vSphere experience, with which customers are familiar. It is supported on a broad choice of DPUs from leading silicon vendors (NVIDIA & AMD) and server designs from OEMs (Dell, HPE).

Distributed Services Engine offloads and accelerates vSphere Distributed Switch and NSX Networking on the DPU, with additional services to follow in the future. So right away, this will benefit customers running applications that demand high network bandwidth and fast cache access such as in-memory databases.

vSphere 8 internal benchmarking study running Redis on a DPU-enabled host achieved 36% better throughput along with a 27% reduction in transaction latency. In another scenario, a DPU-enabled host achieved performance similar to a non-DPU system, with 20% fewer CPU cores. These powerful results show how vSphere 8 enables customers to lower total cost of computing and improve workload performance.

![vSphere8_4](https://user-images.githubusercontent.com/110538923/196092098-f0d51e6c-f216-442a-abcf-4fb8aea357f0.PNG)

Moreover, with vSphere 8 IT admins can reduce operational overhead of operating DPUs in the infrastructure by leveraging integrated vSphere workflows to manage lifecycle and monitor performance.

I am thrilled to note that our technology partnerships have produced market ready end-to-end solutions. Today, Dell Technologies announced the launch of SmartDPU Software Solutions on the VxRailTM   platform with a choice of DPUs from AMD Pensando and NVIDIA. HPE announced the launch of HPE ProLiant with VMware vSphere® Distributed Services Engine™ – based on DPUs from AMD Pensando. VMWare is also excited about the rapid progress of their other partners like Lenovo and Intel are making in bringing more solutions to the market, providing even more choices for their customers.

![vSphere8_5](https://user-images.githubusercontent.com/110538923/196092436-e7eaf835-d626-42b7-8fa9-1855814e3f62.PNG)

When it comes to improving workload performance, vSphere 8 does not stop here. vSphere 8 improves AI/ML model training times and achieves unparalleled levels of performance for the most demanding and complex models by adding support for up to 32 NVIDIA GPUs devices in Passthrough mode – a 4x increase compared to vSphere 7.

![vSphere8_6](https://user-images.githubusercontent.com/110538923/196092604-e8c17099-5c2f-42cf-9068-ce475f705b66.PNG)

Moreover, AI/ML development teams can now achieve higher levels of scalability of available GPU resources with support for up to 8 vGPUs per VM – a 2x increase compared to vSphere 7.

![vSphere8_7](https://user-images.githubusercontent.com/110538923/196092740-b53d3baa-0fab-4b22-97d6-99d9480a443d.PNG)

While Kubernetes has gained widespread adoption as the de-facto container orchestration technology, IT organizations need a simple and easy way to manage containers alongside VMs. That is why VMware created a streamlined Kubernetes management experience that is natively built into vSphere. With vSphere 8, VMware is delivering VMware Tanzu Kubernetes Grid 2.0 – designed to help IT teams and developers address the growing complexity of agile development environments. This latest release of Tanzu Kubernetes Grid adds new flexibility and control for cluster creation, open-source API alignment, and improved application lifecycle management capabilities.

DevOps teams spend a significant amount of time setting up Kubernetes clusters. Even in cases where infrastructure services are readily accessible, they are designed to meet the needs of IT admins and not necessarily integrated with the development environment. As a result, developers either rely on IT admins to provision developer services or standup infrastructure silos to address their needs. With vSphere 8, DevOps teams can now access IaaS services (like provisioning VMs, networking, setting up Tanzu Kubernetes Grid clusters) easily from the new Cloud Consumption Interface service. The Cloud Consumption Interface simplifies infrastructure setup across the vSphere estate through intuitive UIs and developer friendly APIs, freeing up time that can be spent on real development efforts.

![vSphere8_8](https://user-images.githubusercontent.com/110538923/196092918-7f50b292-477e-4d74-92f8-ce0ceb3ed62f.PNG)

![vSphere8_9](https://user-images.githubusercontent.com/110538923/196093080-f1e5e58d-e816-464f-845e-4c8f8cbd24ed.PNG)

With vSphere 8, TKG Availability Zones can be deployed across 3 clusters, which increases the overall resilience of containerized workloads to infrastructure failures. Simplified cluster creation has been made possible thanks a new Cluster API feature called Cluster Class. Users can now create, scale, upgrade and delete clusters, all from a single place. Provisioning, upgrading, and operating multiple Kubernetes clusters is now a simplified, declarative process. Carvel based tooling has been introduced to allow application developers and platform operators to build on Kubernetes with confidence.

![vSphere8_10](https://user-images.githubusercontent.com/110538923/196093265-e64b23e1-86a8-40f1-a737-5af50fd82acb.PNG)

In June of this year, VMWare launched VMware vSphere+, a new offering from the vSphere family, which combines industry-leading cloud infrastructure technology, an enterprise-ready Kubernetes environment, and high-value cloud services to transform existing on-premises deployments into SaaS-enabled infrastructure . vSphere 8 takes these benefits several steps further.

![vSphere8_11](https://user-images.githubusercontent.com/110538923/196093439-b9a23301-fe96-4026-9add-13f679198323.PNG)

With vSphere 8, IT admins can deploy the following add-on cloud services that protect workloads and optimize infrastructure, with more on the way.

VMware Cloud Disaster Recovery add-on service drives resilience of mission critical workloads by protecting them from disasters and ransomware.

![vSphere8_12](https://user-images.githubusercontent.com/110538923/196093600-9409f4c8-fbb9-4f75-a62e-fc55a72209e5.PNG)

![vSphere8_13](https://user-images.githubusercontent.com/110538923/196093738-2d8b0f4b-6709-49d1-8cd9-642ebb30c073.PNG)

![vSphere8_14](https://user-images.githubusercontent.com/110538923/196093844-e680a2e1-64b2-45c3-8b3c-d79deeb6a7a4.PNG)

IT admins spend a lot of time upgrading and maintaining infrastructure. Though regular maintenance operations help ensure uptime and availability, they take time away from running business critical applications. vSphere 8 optimizes maintenance windows by pre-staging ESXi image downloads and performing simultaneous upgrades on hosts, allowing teams to return faster to regular operations.

With the growth of workloads on-premises and at the edge, initial placement and migration are critical aspects that help infrastructure teams maximize service availability, balance utilization, and minimize downtime. vSphere 8 gives a major upgrade to vSphere Distributed Resource Scheduler and vMotion. Distributed Resources Scheduler now factors workload memory usage into placement decisions. It can now place workloads more optimally by taking into consideration memory needs of workloads.

vMotion now supports migration of VMs running on hosts that support Intel Scalable I/O Virtualization (Intel SIOV). Workloads can now simultaneously enjoy the benefits of SIOV passthrough performance and mobility across the vSphere infrastructure.

According to an IDC study, 65% of the global GDP will be digitalized by 2022(4). The IDC study points out the Global Data Sphere is expected to double between 2022 and 2026(5). As the footprint of computing continues to grow, many enterprises are starting to think about sustainable ways to operate infrastructure. VMware has taken the first step in helping enterprises develop sustainable computing strategies. vSphere 8 introduces Green Metrics – that help you track power consumed by workloads and infrastructure operations. This is just the first step in helping customers realize the potential and opportunities to reduce their carbon footprint while meeting business objectives.

![vSphere8_15](https://user-images.githubusercontent.com/110538923/196094078-e156ea04-1ad4-418c-9229-1fb1c522bbfe.PNG)

## About the Author
![ashtechiefinallogo](https://user-images.githubusercontent.com/110538923/196060242-9076fe6b-a236-43b9-bdf7-0d5f1e0b5a8d.png)

I`m Ashish Sharma who brings 24+ Years of Mix & Match Experience of Designing and Architecting Wintel, VMware DCV/NSX/vRO/vRA/vRops, Azure Cloud, Microsoft Cybersecurity, Azure DevOps, AWS, and Google Cloud Solutions offerings.

I am an Expert of Infrastructure as Code using Terraform, Code as Infrastructure (Reverse Terraforming), ARM, Azure Bicep, JSON, AWS CloudFormation, Automation using GitHub Actions, YAML, Jenkins, PowerShell, Azure PowerShell, Configuration Management using Ansible etc. I have very good understanding of Microservices, Containerization aka Open-Source Kubernetes, Docker, Tanzu Grid Cluster and have good knowledge of Scrum, Kanban and other Agile and Project Management tools and methodologies like Microsoft Projects & Jira etc. I am currently exploring “Artificial Intelligence for IT Operations (AIOps)”, specifically Moogsoft.

I do have sound knowledge of Cisco InterSight along with Cisco UCS, Hyperflex, Dell EMC VXRail and other Hyperconverged, Converged & Bare Metal Server Hardware. I have major expertise in Solution Designing of Datacenter and Network Virtualization using VMware vSphere, On-Premises to On-Premises and On-Premises to Cloud Migration & Transformation, Automated & Scripted Migration. I have also taken care of a variety of Greenfield and Brownfield Infrastructure Design, Management, and Security Compliance requirements.

### Contact me

 **⌨️**  [GitHub](https://github.com/ashtechiedevops/) / [LinkedIn](https://www.linkedin.com/in/ashish-sharma-51b3a19/) / [Website](https://ashtechie.com/) / [Twitter](https://twitter.com/ashtechie777/) / [Instagram](https://www.instagram.com/ashtechieworld/)
 











