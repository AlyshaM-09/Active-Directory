  <p align="center">
    <img src="https://github.com/user-attachments/assets/7c9a458b-d110-40bf-82dc-a50291d1bbc8" alt=activedirecotry_logo logo"/>

  
Microsoft Active Directory (AD) is a directory service designed to simplify network management for organizations. Operating on Windows Server, AD efficiently stores and organizes information about network components, including users, devices, and services. It provides convenient access to this information for both administrators and users. Furthermore, AD allows administrators to regulate permissions, manage access to network resources, and create security policies, thus optimizing the overall network management process. <br>

<h2>Technologies used</h2>
-Microsoft Azure <br>
-Remote Desktop <br>
-Active Directory Domain <br>
-PowerShell

<h2>Operating System used</h2>
- Windows 10 <br>
- Windows Server <br>

<h2>Steps setting up in Azure</h2>
In demostration, the NIC in the domain controler need to be set to static. The client computer needs to be set in the same virtual network. There is a seperate section in Azure to create the virtual network. In the clients computer, pull up Powershell and type in ipconfic/ all. Here the DNS should show the Domain Controler IP address. 

<h2>Configuration Steps</h2>
(photo here) <br>
In the Domain Control, download the Active Diretory Domain Services: setup new forest with the domain name (in the work place it can be the company or department name), restart and log back in with the domain name. <br>
(photo here) <br>
Here, create Domain Adim users by creating new Organizational Units. For sake of the tutorial use the name _EMPLOYEES and _ADMIN. The new employee would have their name and permissions listed under _EMPLOYEES or _ADMIN. Log out and log back in as the new employee. <br>
(photo here) <br>
Add the client-1 Virtual Machine into the domain. After restarting, the client-1 should show up in the Active Directory Users and Computers (ADUC). Drag the account to _CLIENTS. Under _CLIENTS will have non admin permissions, by logging into client-1 as admin (mydomain.com/jane_a). <br>

<h2>To learn more in depth of Active Directory:</h2>

### [Microsoft Learning Center](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
