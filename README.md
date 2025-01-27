<p align="center">
<img src="https://i.imgur.com/QNxjap4.png" alt="Permissions Photo"/>


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
<img src="https://i.imgur.com/5di40mj.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/kRfXDoW.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/2vT5VLq.png" height="80%" width="80%" alt="Configuration Steps"/>  
<img src="https://i.imgur.com/Sb8F3U0.png" height="80%" width="80%" alt="Configuration Steps"/>  
<img src="https://i.imgur.com/0XlGPPw.png" height="80%" width="80%" alt="Configuration Steps"/>  


<br />- Log into **dc-1**.
<br />- Choose a random user account previously created. I used bobex.gomo
<br />- Attempt to log in 10 times with an incorrect password.
<br />- Configure Group Policy to lock the account after 5 failed attempts:
<br /> - Follow steps to configure Account Lockout Threshold in Group Policy.
<br />- Attempt to log in 6 times with an incorrect password.
<br />- Observe that the account is locked out in **Active Directory**.
<br />- Unlock the account.
<br />- Reset Password for user bobex.gomo (Right click user name in DC-1, click reset password and reset and unlock for user)
 


</p>
<br />

<p>

</p>
<p>
   
</p>
 

<p>
<img src="https://i.imgur.com/FYAxEiv.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/CmL4aOc.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/08G9pIz.png" height="80%" width="80%" alt="Configuration Steps"/> 
<img src="https://i.imgur.com/QnLUDv1.png" height="80%" width="80%" alt="Configuration Steps"/>  
</p>
<p>

  



<br />- Disable the same account in Active Directory.
<br />- Attempt to log in with the account and observe the error message.
<br />- Re-enable the account.
<br />- Attempt to log in again with the account.  

</p>
<br />

<p>
<img src="https://i.imgur.com/9mpRJWB.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/3nHHp6R.png" height="80%" width="80%" alt="Configuration Steps"/> 
</p>
<p>
<br />


- Observe the logs in the **Domain Controller**.
- Observe the logs on the **client machine**.

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

In this lab, I simulated account lockouts in Active Directory by configuring Group Policy to lock accounts after 5 failed login attempts, then unlocked and reset the account. I also disabled and re-enabled accounts, observing the effects, and analyzed security logs to identify lockout events. Key lessons included balancing security with usability, managing accounts effectively, and leveraging logs for troubleshooting. This hands-on experience highlighted the importance of proper account lockout policies in preventing brute-force attacks while minimizing user disruption.
