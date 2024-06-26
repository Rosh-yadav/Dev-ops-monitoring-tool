
# How to Install Nagios Monitoring Tool


### Steps to be followed:
1.	Updating the packages
- 2.	Installing the latest version of Nagios XI 



**Note**: You need a blank ubuntu lab before you proceed with installations. Any pre-installed tool/package might interfere with the installation process giving errors. So kindly, terminate the lab access and launch a fresh lab instance before you proceed with this demo.


### Step 1: Updating the packages
1.1	Update the packages using the following command:


```
 sudo apt update -y 

```
 
### Step 2: Installing the latest version of Nagios Xi
- 2.1	Login as the root user using the command given below

```
 sudo -i
 
```
 
- 2.2	Execute the below command to install Nagios XI

```
curl https://assets.nagios.com/downloads/nagiosxi/install.sh | sh
```

**Note**: The installation takes around 20 mins. Please wait patiently till you get the Installation Complete message as shown below

 
- 2.3	Navigate to the user interface by using the URL provided in your terminal session. You can refer to the screenshot given above.
- 2.4	You will be presented with the Nagios XI Installation screen as shown below


 

- 2.5	You will be first prompted to define the General System Settings

- 2.6	Once you've made your desired selections choose your License Settings. Here for demonstration purposes we have chosen a trial version. 

- 2.7	You will have to enter a key for the trial version. To get the key, click on the click to get a trial key link. You will be asked to enter details like the first name, last name and email id. Once you enter all those you will get the key mailed to the email-id you just mentioned. Enter the key as shown below
 
- 2.8	Click Next to proceed.

- 2.9	The next page provides you with options for the Admin Account. You can use the default password or change it if you want. After this click on Finish Install
 
- 2.10	The page will display a spinning logo while it applies your settings to Nagios XI.

- 2.11	The Installation Complete screen will be shown with the username and password required to login to Nagios XI.

- 2.12	Click the Login to Nagios XI button to begin.

 

- 2.13	The Login Screen will appear, provide your credentials and then click the Login button.

 

- 2.14	You will need to accept the License Agreement to proceed.
 

- 2.15	You will be logged into Nagios XI and be placed at the home screen.

 


----------------------------------------------------------------------------------------

# Adding Hosts to the Nagios Monitoring Tool


### Steps to be followed:
1.	Logging into the Nagios XI Dashboard
- 2.	Adding a host using the core config manager


### Step 1: Logging into the Nagios Dashboard
1.1	Login to the nagios dashboard using the url as mentioned in the previous demo.
 

### Step 2: Adding a host using the core config manager
- 2.1	Navigate to Configure > Core config manager from the nagios dashboard

 
- 2.2	To manually add a new host, select the Hosts link located under Monitoring on the left menu of CCM
 
- 2.3	This will bring up the Host Management page, which displays a list of the current hosts being monitored by Nagios XI.
 
- 2.4	Click the Add New button to manually add a new host.
 
- 2.5	The Host Management page will open on the Common Settings tab.
 
- 2.6	Define the primary host parameters such as Host Name, Description, Address, and Display name.
 
- 2.7	Use the Manage Parents button to associate parent host(s) for the host.
- 2.8	Use the Manage Templates button to associate template(s) to the host.
 
- 2.9	Use the Manage Host Groups button to associate existing host group(s) to the host
 
 
- 2.10	On the previous screenshot of the Common Settings tab you'll notice that the Active checkbox is checked. If this box is unchecked the host configuration won't be put into production when Apply Configuration is performed. However the settings will remain in CCM until you activate the host object.
 
- 2.11	To define the check command for this host, you select the appropriate command from the Check command drop down list . Every command in the Check command drop down list is associated with a set of Nagios Core commands and arguments, which are shown in the Command view field.

 
- 2.12	The Check Settings tab allows you to specify the settings for frequency of checks and also the host state
 

- 2.13	Configure settings as shown in the screenshot below
 
- 2.14	The Alert Settings tab allows you to specify your notification settings.
 

- 2.15	Enter the value as shown below:
 
- 2.16	Click on manage contacts to add any contact that needs to be notified about the host status.
 
- 2.17	The Misc Settings tab is for defining additional host information
 
- 2.18	Once you've finished entering information for your new host, click the Save button to return to the Host Management page
 
- 2.19	Click the Apply Configuration button to restart Nagios XI and put the new settings info effect. Nagios XI will verify the settings and display a success message that the host was set up correctly
 
- 2.20	You can see the apply configuration successful message as shown below:
 
- 2.21	You can verify that the host is added to the monitoring tool.
 




----------------------------------------------------------------------------------------
