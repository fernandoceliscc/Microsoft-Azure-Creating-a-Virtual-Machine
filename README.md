<p align="center">
<img src="https://azure.microsoft.com/svghandler/virtual-machines?width=600&height=315" alt="osTicket logo"/>
</p>

<h1>Microsoft Azure - Cloud Virtual Machine</h1>
This short tutorial outlines the prerequisites for creating a Virtual Machine within Microsoft Azure on Windows devices <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure Account
- Microsoft Azure Subscription
- Microsoft Azure Resource Group
- Microsoft Azure Virtual Network

<h2>Creation Steps</h2>

<p>
<img src="https://imgur.com/8diR36C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
If you are a first-time Azure user, I recommend starting with the free trial. You'll receive $200 in free credit, but it must be used within 30 days before it expires. During the sign-up process, you'll need to provide typical online payment information for free trials. Rest assured, you will not be charged unless you choose to upgrade your account.

Along with the creation of your account, Azure will provide you with a subscription – a receptacle that holds all the resources created within Azure. Subscriptions come with various pricing options to best match users' needs. It's important to note that the subscription received as part of your free trial is non-customizable.
</p>
<br />

<p>
<img src="https://imgur.com/SN47qhO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will first need to create a Resource Group; this is a container within our subscription used for organizing services and documents. Think of our Tenant (Account) as the Company, the subscriptions as the different departments within the company, and the Resource Groups as the different teams within the departments.

Azure should automatically assign the Resource Group to your free subscription. You can name the resource group 'Virtual_Machine_Project' or choose another name if you have a preference. Select the region closest to your location, skip the tags segment, and then click 'Review and Create.' Enter the Resource Group by either searching for it in the browser or clicking on the Resource Group icon under Azure Services.
</p>
<br />

<p>
<img src="https://imgur.com/2BMGt7F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Once in your Resource Group, select 'Create,' then search for 'Virtual Machine' on the marketplace and click 'Create' on that. Once again, your subscription should default to the free one unless you own another. Your Resource Group should default to the one we just created unless you have made another. Name the virtual machine 'vm-project' or choose another name of your preference.

Ensure your region is the exact same one as your Resource Group; if you can't remember, open a separate tab of Azure and access your Resource Group, which will have the region listed. The Image can be set to Windows 10 Pro, and the size can be the largest one available – in my case, 4 vCPUs with 16GB of memory. The username and password are entirely up to you, but I would recommend making them as simple as possible for this project. If you are creating a virtual machine you plan on using beyond this project, it is at your own discretion.

Skip disks and go to networking. As you can see, a new virtual network will be created alongside your virtual machine using the name you entered for the virtual machine. Creating a second virtual machine under the same region and resource group will give you the option to select the virtual network you are creating now. For this project, we can go straight to 'Review + Create.' The validation should pass with the information we entered. Creating the virtual machine will take Azure a minute or two. You can stay on the deployment page or click the notification tab to see the progress.
</p>
<br />

<p>
<img src="https://imgur.com/8DWGiRl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Enter the Virtual Machine by searching for it in the browser, clicking on the Virtual Machine icon under Azure Services, or accessing it inside your resource group. Once inside, look for the public IP address of the virtual machine and copy it.

Now, click the Windows key and search for 'Remote Desktop Connection,' then open it. In the computer text box, you can paste your virtual machine's IP address. From here, enter the username and password you created for the virtual machine. If the program is trying to log in using your personal account, you can click 'More choices' and then 'Use a different account.' Windows will prompt a security warning; you can click 'Yes.' And that's it! You have created a virtual machine within Microsoft Azure from scratch.
