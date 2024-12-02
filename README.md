# Active Directory Home Lab Part 2: Organizational Units and Groups

<h2>Description</h2>
In this Active Directory Home Lab, I created Engineering, Management, and IT Organizational Units (OUs), created and configured a Group Object file share, and connected a user endpoint to the Group Object file share.   
<br />


<h2>Languages and Utilities Used</h2>

- <b>Windows GUI</b>

<h2>Environments Used </h2>

- <b>Windows Server 22</b> 
- <b>Windows 11 Enterprise</b> 
<br />
<br />
First I created new OUs as Engineering, Management, and IT.

![1) created new OUs for each department](https://github.com/user-attachments/assets/7672e952-1443-4ecc-ab36-6924b1e4d39f)

<br />
<br />
Within the Engineering Ou, I added Bruce Wayne and Dick Grayson Users. 

![2) adding users into OUs](https://github.com/user-attachments/assets/09f7d502-34ca-47a3-bcbf-32020ee4a0a7)

<br />
<br />
Then I created a Group Object called Engineering Share for a file share within the Engineering OU.

![3) creating new engineering group inside engineering OU](https://github.com/user-attachments/assets/256d4f13-0379-4260-a7ad-01c334b7756b)

<br />
<br />
Added users to Group Object Engineering Share.

![4) adding users to engineering group](https://github.com/user-attachments/assets/19dec6a8-966b-4809-9297-8545546ddeab)

<br />
<br />
Created new share folder for Engineering Share. 

![5) creating new share folder for engineering share](https://github.com/user-attachments/assets/8d9221d1-cfd6-485a-8a12-0156228dc191)

<br />
<br />
Confirmed Share name and path to share.

![6) Engineering share name and path](https://github.com/user-attachments/assets/a60cfc88-557a-4108-9d24-f3e42e4f4b3b)

<br />
<br />
Next I customized permissions for the file share.

![7) customize permissions](https://github.com/user-attachments/assets/4e057237-5fde-4a2b-a7d6-f2966c3c9505)

<br />
<br />
Disbaled inheritance and converted inherited permissions into explicit permissions on this group object. 

![8) disable inheritance and convert](https://github.com/user-attachments/assets/eb6579fe-9a22-45ed-bc95-326f68fb5628)

<br />
<br />
Removed users and only left System, Administrators, and Creator Owner in permissions.

![9) remove users ](https://github.com/user-attachments/assets/b9636523-5e1a-4303-ae0b-31db85288d08)

<br />
<br />
Selected Engineering Share Group Object. 

![10) add group engineering share](https://github.com/user-attachments/assets/5c88f81e-bcc5-4e7a-9477-ea64a96aac4a)

<br />
<br />
Make sure to check the write box for basic permissions for Group Object permissions. 

![11) checked box for allow write permissions](https://github.com/user-attachments/assets/ef33fd0f-cf84-4526-8a3d-97daaaf01d8a)

<br />
<br />
Confirmed results in New Share wizard.

![12) create   close](https://github.com/user-attachments/assets/4a015789-2ae3-41e0-8971-8cc77b8f7a3a)

<br />
<br />
Switching over to Windows 11 Enterprise VM as user Batman@GothamCity.local, I began to enable network discovery by logging in.     


![13) logged in as batman to turn on network file sharing](https://github.com/user-attachments/assets/aecbc63e-0f9d-4a0d-9fd6-d2e40266a894)

<br />
<br />
Found the Engineering Share Group Object.

![14) logged in as administrator to allow domain file sharing](https://github.com/user-attachments/assets/b6931d5d-0125-4f29-a4b6-8f0cfcd11fa0)
<br />
<br />
Wrote in the file share "Hello Engineering Share" text file. 

![15) create text file in engineering share as user Batman](https://github.com/user-attachments/assets/d946f5a4-4a74-4042-9073-dd6740478569)

<br />
<br />
Mapped the network drive with the path to the group object Engineering Share for convenience. 

![16) map network share folder for future convenience](https://github.com/user-attachments/assets/9144fbbc-4a1e-4dc9-8d78-80bdfa38cdac)

<br />
<br />
