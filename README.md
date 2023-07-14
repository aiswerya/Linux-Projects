<h1>Software Management</h1>

 

<h2>Description</h2>
In this project, we will  <br />

- <b>Update the Linux machine using the package manager</b> 

- <b>Roll back or downgrade a previously updated package through the package manager</b>

- <b>Install the AWS Command Line Interface (AWS CLI)</b> 
  


<h2>Languages Used</h2>

- <b>Linux</b> 


<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>PuTTy</b>
- <b>AWS Management console</b>
<h2>Procedures</h2>
<h2>Task 1: Use SSH to connect to an Amazon Linux EC2 instance</h2>
In this task, you will connect to an Amazon Linux EC2 instance. You will use an SSH utility to perform all of these operations. <br />

- <b>Select the details drop-down menu and then select show. A Credentials window will be presented. </b>
- <b>Select the Download PPK button and save the labsuser.ppk file. Typically your browser will save it to the Downloads directory. </b>
- <b>Make a note of the PublicIP address. Then exit the Details panel by selecting the X. </b>
- <b>Download PuTTY to SSH into the Amazon EC2 instance. If you do not have PuTTY installed on your computer</b>
- <b>Open putty.exe .Configure PuTTY timeout to keep the PuTTY session open for longer.: Select Connection
Set Seconds between keepalives to 30</b>
- <b>Configure your PuTTY session:
Select Session
Host Name (or IP address): Paste the Public DNS or IPv4 address of the instance you made a note of earlier. Alternatively, return to the EC2 Console and select Instances. Check the box next to the instance you want to connect to and copy the IPv4 Public IP value in the Description tab. </b>

- <b>Back in PuTTY, in the Connection list, expand SSH</b>

- <b>Select Auth (don't expand it). Select Browse</b>

- <b>Browse to and select the lab#.ppk file that you downloaded</b>

- <b>Select Open to select it. Select Open again. </b>

- <b>Select Yes, to trust and connect to the host. When prompted login as enter: ec2-user This will connect you to the EC2 instance. </b>


<h2>Task 2: Update your Linux machine </h2>
In this task, you use the yum package manager to update and upgrade the machine, including relevant security packages. <br />

- <b> To validate that you are in the companyA home folder, enter pwd and press Enter. </b>

- <b> If you are not in this folder, enter cd companyA and press Enter. </b>

- <b> To query repositories for available updates, enter sudo yum -y check-update and press Enter. </b>

- <b> To apply security-related updates, enter sudo yum update --security and press Enter. </b>

- <b> To update packages, enter sudo yum -y upgrade and press Enter.</b>

<p align="center">
ec2-user: <br/>
<img src="https://imgur.com/a/UTpKbdt" height="80%" width="80%" alt="ec2 launching"/>
<br />
<br />





