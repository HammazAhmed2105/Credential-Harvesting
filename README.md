# Credential-Harvesting
<h2>LAb Objective</h2>
Learn how to harvest credentials by utilizing a cloned site
<h2>Lab Tool</h2>
Kali linux in Virtual Machine
We will be using the setoolkit - The Social-Engineer Toolkit (SET) was created and written by Dave Kennedy, the founder of TrustedSec. It is an open-source Python-driven tool aimed at penetration testing around Social-Engineering. 
We will be doing credential harvesting i.e password harvesting or username harvesting, is a form of cyberattack that involves the theft of personal or financial data such as usernames and passwords, typically carried out through phishing, malicious websites, email scams, or malware but not always.
<h2>Download Setoolkit</h2>
Download the tool on your kali linux - git clone https://github.com/trustedsec/social-engineer-toolkit
<h3>Step 1 – Start setoolkit by using the command “sudo setoolkit”. </h3>
<img src="https://i.imgur.com/HMOvawW.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<h3>Step2 – Choose the following options one after another. Social Engineering Attacks > Website Attack Vectors > Credential Harvester Attack Method. Refer to the below image.</h3>
<img src="https://i.imgur.com/3UZnvAc.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<h3>Step 3 - The next menu will ask you which method you want to choose to harvest a victim’s credentials. In this lab we will be cloning a site, so choose option 2.</h3>

<img src="https://i.imgur.com/CXeOkfR.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<H3>Step 4 – Now we have to enter our local machine(Kali linux in this instance) IP address. If you don’t know it then open a new terminal and type “ifconfig”. 
Enter the Ip address and then the web address of the site you wanna clone. I am using Instagram for this example. 
</H3>
<img src="https://i.imgur.com/IozFfxv.png" height=80%" width="80%" alt="Disk Sanitization Steps"/>
<h3>Step 5 -  Go back to any browser and type the IP entered in step 4. You will see a phished Facebook page. Any password and username entered here will go to your kali machine.</h3>
<img src="https://i.imgur.com/zIuXP0W.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<h3>Step- 6 Finally, go back to the terminal where SET is running. You will see lots of text from the numerous POST requests being sent from the cloned site. Scroll down until you see the values username and password. You should be able to see the username and password you entered into the cloned site in cleartext.</h3>
<img src="https://i.imgur.com/ezohMqz.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
