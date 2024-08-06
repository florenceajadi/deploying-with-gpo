<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Deploying A Desktop Background with a GPO</h1>
This tutorial outlines the implementation of deploying a desktop background to your domain with a GPO in Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy A Desktop Background with a GPO](https://youtu.be/cG7M3Z-Cek4)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- 

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Run active directory
- Create a file folder on Windows C drive called 'Desktop Backgrounds'
- Share and permit folder with other users
- Create a new GPO called 'Desktop Backgrounds'
- Enable Wallpaper change 
- Using command prompt to verify change is accurate
- Log in to see new wallpaper



<h2>Deployment and Configuration Steps</h2>

<p>
<img src="" height="80%" width="80%""/>


</p>
<p>
Diagram
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/605b9268-b7be-40ba-9ed7-a4d0f8f9c96d" height="80%" width="80%""/>


</p>
<p>
Created a File Folder on Windows :\C drive called Desktop Backgrounds.
</p>
<p>
  <img src="https://github.com/user-attachments/assets/b91522ce-2590-487a-bbb9-761a930c3afe" height="80%" width="80%""/>
</p>
<p>Created an advanced sharing permission on Desktop Backgrounds folder for Authenticated Users with only read access. </p>
<br />

<p>
  <img src="https://github.com/user-attachments/assets/71ec2dc2-d9d9-48d9-bc37-d6d36c7b8897" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/527498af-82b4-40f3-ac15-557d75717e5d" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/7242ee43-233e-4afc-b4ae-9230cdb04dfc" height="80%" width="80%" />




</p>
<p>
Created a new GPO called Desktop Backgrounds within mycybercat.com domain. Enabled Desktop Wallpaper and linked the url from the my local network server (ADG-vm), with the file folder we created unto the Wallpaper Name.
</p>
<br />

<p>
 <img src="https://github.com/user-attachments/assets/d8b85aa5-fff6-420d-aed2-0da6c45d447c" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/086f8d6f-4d79-4e4f-8c42-79a13293bef5" height="80%" width="80%""/>
</p>

<p>
Used gpupdate /force on command prompt to check updates.
</p>
<p>
  <img src="https://github.com/user-attachments/assets/d9213a77-6892-43fa-ad6b-7063707862a4" height="80%" width="80%""/>
</p>
<p>Used gpresult /r on command prompt to see if our Group Policy Object is updated with Desktop Background. As You can see, it is.</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/577cab8e-851f-4358-a37b-4bad0d35a34f" height="80%" width="80%""/>

</p>

  
<p>
My Screen Wallpaper is now CYBERGIRL.com </p>
<p>
  <img src="" height="80%" width="80%""/>
</p>

<p>
    Jeremy Collins is now added to the Sales group. We can even look into Jeremy Collins' account to see who is a member of. 

</p>
