# Active-Directory-Account-Security

</p>


<br /><h2>Objectives</h2>
This project demonstrates the implementation and management of account security in an Active Directory environment. It focuses on configuring account lockout policies, managing account states, and monitoring event logs for security operations, laying the groundwork for cybersecurity practices. <br />

<h2>Skills</h2>

<br />-Active Directory Management
<br />-Group Policy Configuration
<br />-Security Policy Enforcement
<br />-Log Analysis and Monitoring
<br />-Troubleshooting and Issue Resolution

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
  

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 Pro (21H2)

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/zo0BWbb.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/EHU2ooS.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/arbzQKI.png" height="80%" width="80%" alt="Configuration Steps"/>  
</p>
<p>

<br />- Log into **dc-1**.
<br />- Choose a random user account previously created.
<br />- Attempt to log in 10 times with an incorrect password.
<br />- Configure Group Policy to lock the account after 5 failed attempts:
<br /> - Follow steps to configure Account Lockout Threshold in Group Policy.
<br />- Attempt to log in 6 times with an incorrect password.
<br />- Observe that the account is locked out in **Active Directory**.
<br />- Unlock the account.
<br />- Reset the password.
<br />- Attempt to log in again with the new password. 


</p>
<br />

<p>

</p>
<p>
   
</p>
 

<p>
<img src="https://i.imgur.com/YtUCCF9.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/q0tdWdI.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/URuAmsO.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>

  



<br />- Disable the same account in Active Directory.
<br />- Attempt to log in with the account and observe the error message.
<br />- Re-enable the account.
<br />- Attempt to log in again with the account.  

</p>
<br />

<p>
<img src="https://i.imgur.com/8FUGk5N.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
<br />


<br />- Enable Remote Desktop for non-administrative users <br />
<br />- Log in as an administrator (e.g., Jane).  
<br />- Open **System Properties** and click on **Remote Desktop**.  
<br />- Select users that can remotely access the PC.  
<br />- Allow **Domain Users** access to Remote Desktop.  
<br />- Non-administrative users can now log in to the client computer.  
<br />- Note: Group Policy can be used to apply this change across multiple systems, but it is not used in this lab.  
</p>
<br />

<p>
<img src="https://i.imgur.com/h9c3YOM.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/xalP6Gh.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>

<br />- Users can be created manually or with a script.<br />  
<br />- For this lab, a PowerShell script is used.<br />  
<br />- Log in to the domain controller with an admin account.<br />  
<br />- Open **PowerShell ISE** as an administrator.<br />  
<br />- Create a new file and paste the script into the ISE console.<br />  
<br />- Run the script and observe the accounts being created.<br />  
</p>

<p>
<img src="https://i.imgur.com/499JIxw.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>
<p>
<br />- Users created with the PowerShell script can now sign in to Client-1.  
<br />- Observe that in Active Directory, under -Employees users are created.  
<br />- User are able to be log into Client-1 with password1.
</p>
<br />

<h2>Lessons Learned</h2>

Completing this lab has taught me how to set up Active Directory and join client machines to the domain. I also learned how to create users and assign the necessary permissions. Although Active Directory involves a lot of menu navigation, it is not difficult to grasp. This lab serves as a gateway for me to explore DNS settings and file permissions in greater depth, which I will cover in future labs.
