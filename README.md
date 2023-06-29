<p align="center">
<img src="https://i.imgur.com/1DDZ4Ui.png" height="50%" width="50%" alt="Microsoft Azure Logo"/>
</p>
<p align="justify">

<h1>Create an Azure Account and Deploy a Virtual Machine</h1>
Microsoft Azure is a cloud computing platform with numerous products and services. This guide will demonstrate how to create an account, utilize the portal, and create a virtual machine.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure
- Microsoft Remote Desktop (macOS) for virtual machines

<h2>Configuration Steps</h2>

<h3>Create a "FREE" Azure Account</h3>

Go to [https://azure.microsoft.com/en-us/free/](https://azure.microsoft.com/en-us/free/)
- Click "Start Free".
- Follow the prompt to create an account.
  - You <b>will</b> need to put in your credit card information to receive the free $200 worth of Azure credits!
    <div> It will not charge you until the $200 credits runs out or the account has been active for a <b>30 days</b>.
- Once completed, click on <a href="https://portal.azure.com/">Go to the Azure Portal (portal.azure.com)</a>.

<p align="center">
<img src="https://i.imgur.com/GRuFyfG.png" height="64%" width="64%" alt="Azure Free Account"/>
</p><hr>

<h3>Create a Resource Group</h3>

- In the Search Box at the top header, type and select "Resource groups".
  - If "Resource groups" is already listed on the front page, then you can simply click on it, rather than manually searching.
<p align="center">
<img src="https://i.imgur.com/gza489d.jpg" height="64%" width="64%" alt="Azure Step 2-1"/>
</p>

- Click "Create" on the top left menu, OR press "Create resource group" in the center box.
<p align="center">
<img src="https://i.imgur.com/5Jo1cEg.jpg" height="64%" width="64%" alt="Azure Step 2-2"/>
</p>

- Name your "Resource group" to whatever you want (e.g. **RG-01**).
- Change the "Region" to a location that is closest to you (e.g. **(US) West US 3**).
- Skip everything else and click "Review + Create" on the lower left.
- Once "Validation passed" on the next page, click "Create".
<p align="center">
<img src="https://i.imgur.com/PCeEU79.png" height="100%" width="100%" alt="Azure Step 2-3"/>
</p><hr>

<h3>Create a Storage Account</h3>

- In the Search Box at the top header, type and select "Storage accounts".
  - If "Storage accounts" is already listed on the front page, then you can simply click on it, rather than manually searching.
<p align="center">
<img src="https://i.imgur.com/HMUaR98.jpg" height="70%" width="70%" alt="Azure Step 3-1"/>
</p>

- Click "Create" on the top left menu, OR press "Create Storage accounts" in the center box.
<p align="center">
<img src="https://i.imgur.com/sGDY2Im.jpg" height="70%" width="70%" alt="Azure Step 3-2"/>
</p>

- Use the same resource group that was just created (e.g. **RG-01**).
- Create a unique name for the storage account that hasn't already been taken (e.g. **saname01**).
- Choose the same region (e.g. **(US) West US 3**).
- Skip everything else and click "Review", then "Create".
<p align="center">
<img src="https://i.imgur.com/07sG8Z6.jpg" height="100%" width="100%" alt="Azure Step 3-3"/>
</p><hr>

<h3>Create a Virtual Machine</h3>
     
- In the Search Box at the top header, type and select "Virtual machines".
  - If "Virtual machines" is already listed on the front page, then you can simply click on it, rather than manually searching.
<p align="center">
<img src="https://i.imgur.com/6DdH3MD.jpg" height="70%" width="70%" alt="Azure Step 4-1"/>
</p>

- Click "Create", then select "Azure Virtual Machine"
<p align="center">
<img src="https://i.imgur.com/tiC5aA4.jpg" height="70%" width="70%" alt="Azure Step 4-2"/>
</p>

- Use the same resource group (e.g. **RG-01**)
- Name your virtual machine however you want (e.g. **virtualmachine01**)
- Use the same region (e.g. **(US) West US 3**)
- Choose your "Image" (e.g. **Windows 10 Pro, version 22H2 - x64 Gen2**)
- Choose a "Size" (e.g. **Standard_E2s_v3 - 2 vcpus, 16 GiB memory**)
- Create any username and password of your choice (this example uses the username: **vmuser**)
  - Make sure NOT to forget these credentials.
- Check the "Licensing" checkbox.
- Click "Review + create".
  - Once "Validation passed" on the next page, click "Create".
<p align="center">
<img src="https://i.imgur.com/UaviYRo.jpg" height="70%" width="70%" alt="Azure Step 4-3"/>
<img src="https://i.imgur.com/mcix7TW.jpg" height="70%" width="70%" alt="Azure Step 4-4"/>
</p><hr>

<h3>Connect to the Virtual Machine via Remote Desktop</h3>

- Go to your Virtual Machine that was just created and "Copy" the public IP address (located on the right side).
<p align="center">
<img src="https://i.imgur.com/Cr02uvs.jpg" height="100%" width="100%" alt="Azure Step 5-1"/>
</p>

- Press the Windows Key (or Start Button), type and select "Remote Desktop Connection".
- Input the virtual machine's Public IP Address and click Connect.
- Enter the username and password from the Step above, then click OK.
  
<p align="center">
<img src="https://i.imgur.com/2Ec29dX.png" height="64%" width="64%" alt="Azure Step 5-2"/>
</p>

- Macintosh users will have to take a different approach:
  - Download "Microsoft Remote Desktop", and Open it.
- Click "Add PC", input the public IP address, then select "Add".
<p align="center">
<img src="https://i.imgur.com/ZhWBhLs.png" height="50%" width="50%" alt="Azure Step 5-2-1"/>
<img src="https://i.imgur.com/Mx1gHxa.png" height="50%" width="50%" alt="Azure Step 5-2-2"/>
</p>
  
- Double-click on the virtual machine, then enter the username and password from the Step above.
- Select "Continue".
- A prompt will appear about the identity cannot be verified; just click "YES".
<p align="center">
<img src="https://i.imgur.com/3YxlS2G.jpg" height="64%" width="64%" alt="Azure Step 5-3"/>
</p>

- Toggle any settings you want, then click "Accept".
<p align="center">
<img src="https://i.imgur.com/VlNH4O9.jpg" height="50%" width="50%" alt="Azure Step 5-4"/>
</p>
<br>

<h2 align="center">
🎇CONGRATULATIONS!🎇
  <br>
You have created your first virtual machine within Azure!
</h2>
  
<p align="center">
<img src="https://i.imgur.com/PpLmQO7.jpg" height="80%" width="80%" alt="Azure Step 5-5"/>
</p>
<hr>

<h2 align="center">
🛑REMEMBER TO DELETE YOUR RESOURCES ONCE YOU ARE DONE WITH THE LAB🛑
</h2>
