<p align="center">
<img src="https://camo.githubusercontent.com/f8ede6a7f4ad832bfd66a54f6912689d1ef080eb15e2b64b7ca43306d648395d/68747470733a2f2f696d6775722e636f6d2f4f7771396c4f562e706e67" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
<p align="center">~This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.~</p>


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Applied</h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Links (to be used inside your VM):</h2>
<li>Help Desk Login Page: http://localhost/osTicket/scp/login.php</li>
<li>End Users osTicket URL: http://localhost/osTicket/</li>
</h2>

<h2>Creating a Ticket</h2>
<li>Within the VM (virtual machine):<br>     Open a browser and paste in the Users OsTicket URL: http://localhost/osTicket/</li>
<li>Click on "Open a New Ticket"</li>
<img src="https://imgur.com/CZZ6qvX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<h2>Karen (bank manager)</h2>
<li>Create a Ticket as Karen with a Help Topic: "Business Critical Outage"</li>
<li>For Issue Summary * type: Entire mobile online banking is down.</li>
<li>In the Details section type: "Multiple clients are reporting they are getting a 404 error when attempting to sign into their account."</li>
<li>When finished, at the bottom click "Create Ticket"</li>
<img src="https://imgur.com/WpORftR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
<p>
  <h2>Ken (in accounting)</h2>
Click "Open a New Ticket" and create a ticket as Ken
<img src="https://imgur.com/EhDfWIf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<li>Make the Help Topic: "Personal Computer Issues"</li>
<li>For Issue Summary * type: Accounting Dept Adobe Reader Not Working</li>
<li>In the Details section type: <br>
"Following the upgrade last night, Adobe Reader has been unusable for all members of the accounting team."</li>
<li>When finished, at the bottom click "Create Ticket"</li>
<img src="https://imgur.com/8Iktzrw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Karen (2nd inquiry)</h2>
<li>Open a New Ticket as Karen with a Help Topic of "General Inquiry"</li>
<li>For Issue Summary * type: When are we getting new hardware</li>
<li>In the Details section type: <br>
"Most of my department are having issues with their tablets. We need new ones ASAP.
Can you provide info?"
<li>When finished, at the bottom click "Create Ticket"</li>

<img src="https://imgur.com/ngWxa2C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Responding to Tickets:</h2>
<li>Log out of osTicket and sign back in as Agent, Jane Doe</li>
<img src="https://imgur.com/VM0Tpq7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Que Manager/Escalation Engineer</h2>
<li>Here you will perform a triage of sorts and assess and assign jobs</li>
<img src="https://imgur.com/UJJCYds.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<li>Let's start with the ticket that reads: "Entire mobile online banking is down."</li>
<li>After reading the notes it's decided that the Priority should be changed from "Normal" to "Emergency" </li>
<img src="https://imgur.com/W1BXeWp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<li>Since Jane is also wearing the Escalation Engineer hat, she assigns it to herself to over see the ticket personally.</li>
<img src="https://imgur.com/2LTGaTp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
<li>Next she addresses the SLA Plan to make it refelect the Emergency by changing it from "Default SLA" to "SEV-A"</li>  
<img src="https://imgur.com/ntxEbeA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<li>System Administrators are more likey to be responsible this type of event.<br> Change the Department from "Support" to "System Administrators"</li>
<img src="https://imgur.com/QN3fL3m.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<li>Notice the Ticket Thread/History showing all the updates</li>
<img src="https://imgur.com/3M0ZOSu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<li>Post a reply: Coordinating with Sys Admin Team to bring mobile banking back online.</li>
<img src="https://imgur.com/4XKLc10.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>

<li> Post a final response: Jullian from Sys Engineering found and corrected a load balancer.<br>
Mobile banking should be operational again.</li>
<li>Mark the Ticket Status "Resolved" and click Post Reply</li>
<img src="https://imgur.com/oCQNBC6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br>
<li>The next ticket we'll address is Ken's ticket for the accounting department</li>
<li>Although this ticket may not be critical or an emergency <br>
the entire accounting department's work is impacted so let's set the Priority to "High" and click "Update"</li>
<img src="https://imgur.com/4qzRACv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<Because it's the whole department, update the SLA Plan to "SEV-B">
<li>Assign this Ticket to John Doe</li>
<img src="https://imgur.com/W6KIrvq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<li>We can now add notes such as, "Reassigned to SEV-B. Reached out to John for a warm handoff." (Post Reply)<br>
In this case a warm handoff is calling and getting an acknowledgment rather than just assigning it (cold handoff).</li> 
<img src="https://imgur.com/YcCD6zB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
           
<br>
            
NOTE: Things like SLA and Priority are determined by the organization which will usually give guidelines to be utilized.
            
<br>
            
<li>Going back to "Tickets" Let's look at Karen's second Ticket "When are we getting new hardware"</li>
<li>Set Priority to "Low"</li>
<li>Assign to yourself (as Jane Doe)</li>
<li>SLA Plan: SEV-C</li> 
<img src="https://imgur.com/NoqchAe.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
<li>In the Response section type something like this: <br>
"Just to update you, we have planned a hardware refresh in Q1 and would like to extend an invitation to you and your department to start testing the new units today, if you are interested. If you wish to proceed, kindly send me an email and let me know."</li>   
<li>Change "Ticket Status" to "Resolved" and click "Post Reply" to close this ticket, removing it from the que.</li>
<img src="https://imgur.com/dl6Jnlz.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<br>
                                                
<li>The only remaining ticket is assigned to John Doe. Sign out and sign back in as John.</li>
<li>John post an internal note that he has rolled back the version of Adobe so they can resume work <br> 
    until he can research why the new version is not working on accounting department hardware.</li>
<li>If you have any trouble posting as John be sure to check the permissions assigned to him.</li>                                                
