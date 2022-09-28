<h1>Azure Sentinel Map </h1>


<h2>Project Overview</h2>
Azure Project Write Up
This blog post is about I project I recently completed where I setup Azure and Microsoft Sentinel with a virtual machine to act as a honeypot to monitor the various attacks that came from different countries and IP addresses. I didn’t have any previous experience with Azure or Sentinel beforehand, so this project taught me a ton. This isn’t going to be an exact step by step walkthrough of how the project is supposed to be, but more of an overview of the project as well as the main things I learned while completing it. I will add the YouTube video tutorial at the end so you can try it out as well!

To start, this components needed to complete this project included an Azure account ($200 free credit), virtual machine in Azure where we purposely turn off the external and Windows firewall to attract attackers, a log repository in Azure called Log Analytics Workspace which is used to ingest the logs from the virtual machine, Microsoft Sentinel (Microsoft’s SIEM) to create a map to visualize where the attacks are coming from worldwide, and PowerShell to extract the IP address from the Windows log to create a custom log using a third-party API. 

While completing this project, it forced me to learn the ins and outs of Azure to a point where I’m comfortable using the cloud platform. From previous experience, I’ve noticed that by just learning where everything is and understanding the terminology of a specific platform is the first step towards mastery. The most interesting part of the project in my opinion was the fact that you can create custom logs in Azure by using the custom PowerShell script with the third-party API. The third-party API used in this project was ipgeolocation.io and the site’s main purpose was to obtain useful information for the logs such as latitude, longitude, state/province, etc. I was also intrigued by how quickly and rapidly attackers were trying to hack into the honeypot. After only 24 hours, there were up to 17,000 attempts at hacking into the virtual machine. Majority of the attacks came from Vietnam and Panama.

In all, I thoroughly enjoyed this project, and I would highly recommend it to anyone looking to gain experience in using Azure and Sentinel. Completing this project is also an eye opener on just how often potential attacker are looking for vulnerable systems. Whether they’re actual people or bots, it’s important to make sure your system is always protected. Below I will include screenshots of certain aspects of the project. The link to this project is: https://youtu.be/RoZeVbbZ0o0 


 


<h2>Log Analytics Workspace </h2>
<img src="https://i.imgur.com/Jyjlk0Z.jpg" height="60%" width="60%" alt="Disk Sanitization Steps"/>


<h2>PowerShell Script</h2>
<img src="https://i.imgur.com/UHflurP.jpg" height="60%" width="60%" alt="New Scan"/>

<h2>Virtual Machine</h2>
<img src="https://i.imgur.com/qPhePXQ.jpg" height="60%" width="60%" alt="New Scan"/>

<h2>Log Analytics Workspace Logs</h2>
<img src="https://i.imgur.com/x286Xai.jpg" height="60%" width="60%" alt="New Scan"/>

<h2>Sentinel Overview</h2>
<img src="https://i.imgur.com/sfMhVUg.jpg" height="60%" width="60%" alt="New Scan"/>

<h2>Failed RDP Map</h2>
<img src="https://i.imgur.com/ClUtUuJ.jpg" height="60%" width="60%" alt="New Scan"/>



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
