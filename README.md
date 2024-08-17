<h2>Creating our insecure Virtual Machines</h2>

To begin working inside the Azure Honeynet project, we'll first need set up the virtual machines we're going to use. These VM's will be the foundation of all our projects and labs. 

First, you'll need to create a virtual machine. Which you can do by visiting [This](link) link

<h2>Security metrics measurement:</h2>

<p align="center">
Secondly, we'll create the virtual machines. 
  <br/> 
<img src="https://i.imgur.com/ApfLPyM.png" height="10%" width="50%" alt="NSGALLOW"/>
<br />
<br />

<img src="https://i.imgur.com/gmqVNNI.png" height="10%" width="50%" alt="NSGALLOW"/>
<br />
<br />

<p align="center">
Continuing the creation of the VM, I assign the correct resource groups and settings. As the only use of this VM is going to be used for the honeynet, I don't need and form of avalability. We will also be leaving the Networking setting to their defaults.
  <br/> 
<img src="https://i.imgur.com/bZuGWcr.png" height="10%" width="50%" alt="NSGALLOW"/>
<br />
<br />

<p align="center">
Finally, we'll configure the VM's Network security groups settings. 
  
 To do this, We'll use the Azure portal we'll search for "Network security groups" Once there, select your VM you would like to edit the NSG of.

 Once in the NSG gettings, you'll find a section for "Inbound Security rules", Which is where you control what kind of traffic is allowed to reach the VM. Click on "add" to create a new rule.

 For the source port, we leave it on "any" to allow all traffic to flow from all sources.

 For port ranges, we want all ports open so there is no traffic that is restricted what-so-ever. Same with Protocals.

 We set the priority of this rule the highest, The lower the priority number, the higher the priority actually is, by setting it to a number lower than any other rules in our NSG

 <p align="center">
  <br/> 
<img src="https://i.imgur.com/GDkwb0d.png" height="10%" width="50%" alt="NSGALLOW"/>
<br />
<br />

<p align="center">

After reviewing all the settings, click on "add" to create the rule!

<h2>Conclusion</h2>
By creating the VMs with an open inbound security rule, we're leaving VM open for all traffic, positive and negative. 
This allows us to attract attackers and observe their actions in a controlled environment.

