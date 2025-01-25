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


- Observe the logs in the **Domain Controller**.
- Observe the logs on the **client machine**.
- Visit **joshmadakor.tech/cyber** for a precursor to cybersecurity and security operations. 
</p>
<br />

<p>

</p>


</p>

<p>

</p>
<p>

</p>
<br />

<h2>Lessons Learned</h2>

Completing this lab has taught me how to set up Active Directory and join client machines to the domain. I also learned how to create users and assign the necessary permissions. Although Active Directory involves a lot of menu navigation, it is not difficult to grasp. This lab serves as a gateway for me to explore DNS settings and file permissions in greater depth, which I will cover in future labs.
