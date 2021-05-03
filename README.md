# IT-Glue
Scripts for documenting 365 data into IT Glue

# Intune Devices

Document all devices enrolled into Intune as a new Flexible Asset. The script creates new devices or updates existing devices so that you can run this script periodically. Document the following:
<ul>
 	<li><strong>Device Name</strong></li>
 	<li><strong>Ownership (Corporate or Personal)</strong></li>
 	<li><strong>OS</strong></li>
  <li><strong>OS Version</strong></li>
  <li><strong>Compliance State</strong></li>
  <li><strong>User</strong></li>
  <li><strong>Autopilot Enrolled</strong></li>
  <li><strong>Encrypted</strong></li>
  <li><strong>Serial Number</strong></li>
  <li><strong>Configurations(if existing)</strong></li>
</ul>
<div>All devices are listed for the customer as a new flexible asset.</div>
<br>
<a target="_blank" href="/Images/pic5.png">
<img src="/Images/pic5.png" alt="Download SPPKG file screenshot" style="max-width:100%;">
</a>
<br>
<a target="_blank" href="/Images/pic4.png">
<img src="/Images/pic4.png" alt="Download SPPKG file screenshot" style="max-width:100%;">
</a> 

<h2>Prerequisites</h2>
You will need to garner tokens and GUIDs from both the Secure Application Model and Syncro. The secure application model allows for a headless connection into all of your customer environments. The script to run that can be found from Kelvin over at CyberDrain. <a href="https://github.com/KelvinTegelaar/SecureAppModel/blob/master/Create-SecureAppModel.ps1">Click here to go to that page in Github.</a>
<br></br>
In IT Glue you will need to create a new API Key. <a href="https://support.itglue.com/hc/en-us/articles/360004938078-Getting-started-with-the-IT-Glue-API">Click Here for IT Glue's Documentation on generating a new API key</a>.
<br></br>
In Microsoft, you will need to make sure you add the following permissions from the ap that was created with the Secure Application model if they are not already there:
<ul>
<li>DeviceManagementConfiguration.Read.All</li>
<li>DeviceManagementManagedDevices.Read.All</li>
</ul>
Reference <a href="https://support.itglue.com/hc/en-us/articles/360004938078-Getting-started-with-the-IT-Glue-API">the following documentation</a> for steps on adding permission to your app registration. 

<h2>Author(s)</h2>
Nick Ross
