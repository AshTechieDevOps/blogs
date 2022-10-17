## Using System file check (SFC) Scan and Repair System Files and to use  DISM to fix the things that SFC cannot.

Written By Ashish Sharma | Oct 17, 2022
Categories: Windows, System File Checker, Windows OS Deployment Image Cleanup and Restore

## Summary

System file check is a utility built into the Operating System that will check for system file corruption The sfc /scannow command (System File Check) scans the integrity of all protected operating system files and replaces incorrect, corrupted, changed, or damaged versions with the correct versions where possible.  When it cannot repair the damage DISM should be run to fix as many errors as possible.

## To run a system file check (SFC)

-   Go to start>Type CMD

-   Right click and run as Administrator

-   (called an elevated command prompt)

-   If you want to verify and repair the OS type sfc /scannow (note the space between sfc and "/")

-   If you just want to check (verify only) the OS type sfc /verifyonly (no changes will be made using verify only)

## When you have finished it will say one of three things

-   Windows did not find any integrity violations (a good thing)

-   Windows Resource Protection found corrupt files and repaired them (a good thing)

-   Windows Resource Protection found corrupt files but was unable to fix some (or all) of them (not a good thing)

## If you get this message run DISM as shown as  below:-

<img width="435" alt="sfc1" src="https://user-images.githubusercontent.com/110538923/196187865-5fc42994-264a-4322-955a-1153f507a6fd.PNG">

## If SFC was not able to repair some or all of the files there are a few options including a repair install from the OS dvd, and DISM. And If SFC did not find any violations it is still a good idea to run DISM Restorehealth to check, scan and restore the health to fix the issue. By using DISM you can run Check, then Scan, but you should always run RESTORE HEALTH at the end to fix the issue.

## To check the health (You would use /CheckHealth to only check whether the image has been flagged as corrupted)

-   run Dism /Online /Cleanup-Image /CheckHealth

## To scan the health use /ScanHealth to scan the image for component store corruption. This option does not fix any corruption.

-   run Dism /Online /Cleanup-Image /ScanHealth

## To RESTORE health (recommended)

-   Use DISM /Online /Cleanup-Image /RestoreHealth to scan the image for component store corruption, perform repair operations automatically, and records that corruption to the log file.  This generally takes 15-30 minutes depending on the corruption and size of the partition.

## You can run scanhealth & restore health at the same time like shown in below:-

-   DISM.exe /Online /Cleanup-image /Scanhealth && DISM.exe /Online /Cleanup-image /Restorehealth

-   If you want to execute Restorehealth as a separate command, the Type "DISM /Online /Cleanup-Image /RestoreHealth" and hit enter.

<img width="440" alt="dism1" src="https://user-images.githubusercontent.com/110538923/196190160-136cb9e5-a04c-43d8-af26-c713686c2779.PNG">

-   If you get the error message "cannot find source files"you need to have an ISO file mounted and need to specify where it is located with the below command. The ISO must be exactly the same version as the running OS.  An ISO of 10586.0 will not repair a running system of 10586.35 because it has additional updates and files.

-   Usee the following command "DISM /Online /Cleanup-Image /RestoreHealth /source:WIM:X:\Sources\Install.wim:1 /LimitAccess"  Where "X" is the drive letter where the ISO is located.  Simply change the "X" to the correct drive letter.

-   If the repair is successful you may want to re-run SFC just to crosscheck if everything is OK because after running DISM it is a good idea to re-run SFC /scannow to make sure all the issues were fixed.


## About the Author

![ashtechiefinallogo](https://user-images.githubusercontent.com/110538923/196060242-9076fe6b-a236-43b9-bdf7-0d5f1e0b5a8d.png)

I`m Ashish Sharma who brings 24+ Years of Mix & Match Experience of Designing and Architecting Wintel, VMware DCV/NSX/vRO/vRA/vRops, Azure Cloud, Microsoft Cybersecurity, Azure DevOps, AWS, and Google Cloud Solutions offerings.

I am an Expert of Infrastructure as Code using Terraform, Code as Infrastructure (Reverse Terraforming), ARM, Azure Bicep, JSON, AWS CloudFormation, Automation using GitHub Actions, YAML, Jenkins, PowerShell, Azure PowerShell, Configuration Management using Ansible etc. I have very good understanding of Microservices, Containerization aka Open-Source Kubernetes, Docker, Tanzu Grid Cluster and have good knowledge of Scrum, Kanban and other Agile and Project Management tools and methodologies like Microsoft Projects & Jira etc. I am currently exploring “Artificial Intelligence for IT Operations (AIOps)”, specifically Moogsoft.

I do have sound knowledge of Cisco InterSight along with Cisco UCS, Hyperflex, Dell EMC VXRail and other Hyperconverged, Converged & Bare Metal Server Hardware. I have major expertise in Solution Designing of Datacenter and Network Virtualization using VMware vSphere, On-Premises to On-Premises and On-Premises to Cloud Migration & Transformation, Automated & Scripted Migration. I have also taken care of a variety of Greenfield and Brownfield Infrastructure Design, Management, and Security Compliance requirements.

### Contact me

 **⌨️**  [GitHub](https://github.com/ashtechiedevops/) / [LinkedIn](https://www.linkedin.com/in/ashish-sharma-51b3a19/) / [Website](https://ashtechie.com/) / [Twitter](https://twitter.com/ashtechie777/) / [Instagram](https://www.instagram.com/ashtechieworld/)
 
