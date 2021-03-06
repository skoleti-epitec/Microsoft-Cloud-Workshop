# Introduction

# Sign-up for Workshop Environment

To make it easier for you to work on the labs, you are provided with pre-provisioned Azure environment. You will receive sign-up link for the lab environment from your instructor. 

* Register for the lab environment by providing your information and clicking on **Submit** button.

* On the next page, click the **Launch Lab** button.
 
* Wait for the lab environment to be provisioned. Sometimes this can take upto **10 minutes**. Once environment provisioning is complete, you will receive details in email as well as in the browser.
 
 > Note: Lab environment is enabled only for specific duration or workshop end time - whichever is earlier. At the end of the allowed time, environment will be self-destructed. Also, for multi-day workshops, all virtual machines will be shutdown at 7 PM local time and start at 8AM local time.

# Verify the pre-provisioned Environment

* Users can use the **Azure Credentials** given to them to login to the Azure Portal
* Two resource groups **ODL_mca-XXXXX-01** and **ODL_mca-XXXXX-contososports** will be already created. In resource group **ODL_mca-XXXXX-01** you will get Azure Environment with the LABVM deployed in it.
* Users can select **labvm** and click on **Connect** to download the RDP file
* Open the RDP file to connect to the LABVM. Provide the credentials you received to login to the VM
* Once you login to the LABVM, server manager will open. Select Local Server and verify that IE Enhanced Security Configuration has also been turned off 
* Go to C:\Hackathon folder and verify application files are there such as:
```
Contoso.Apps.SportsLeague.Web 
Contoso.Apps.SportsLeague.Admin 
Contoso.Apps.SportsLeague.Data 
Contoso.Apps.SportsLeague.Offers 
Contoso.Apps.PaymentGateway 
```
* Also verify that SQL Server Management Studio is installed 

## Verify Azure Access

Open a browser instance in private or incognito mode and login to [Microsoft Azure Portal](https://portal.azure.com) using the credentials provided.

> Note: You might have an existing Azure Credential. For the pre-provisioned environment, new Microsoft Azure environment is provisioned and new AAD user is created for you. To prevent conflict with your existing accounts, it is advised to use In Private mode of IE / IE Edge or Incognito mode of Chrome browser.

## Verify Virtual Machine

You are provided a Visual Studio Community 2017 on Windows Server 2016 (x64)Microsoft with additional softwares configured. FQDN of the LABVM virtual machine and administrator credentials are provided in the lab details page. You can remote into the virtual machine using the provided credentials

# Notes to Attendees
You can use **ODL_mca-XXXXX-contososports** resource group for deploying all the resources in this lab.</br>
While doing Exersice 4, please follow the below steps.
* In Task 1 > Subtask 2, instead of Steps 3, 4 & 5, do the following:
    * In **Usage** menu click on **Impact**.
    * In the new page that appear, click on **Get Started**.
    * Copy the full contents of the JavaScript.
    * Continue with Step 6.</br>
* You can skip Exercise 5.

# Known Issues

### Connecting DSVM with RDP having issue addresses CredSSP

> **Possible Solutions**:

* With the release of the March 2018 Security bulletin, there was a fix that addressed a CredSSP, “Remote Code Execution” vulnerability (CVE-2018-0886) which could impact RDP connections. 
**Resolution**
Please follow the instruction under https://github.com/SpektraSystems/Microsoft-Cloud-Workshop/blob/master/RDP%20CredSSP/README.md

# Notes to Instructors / Proctors

* LABVM is already deployed in **ODL_bcdr-XXXXX-01** Resource Group and configured with all the requirements such as SQL Server Management Studio and Application Files are already downloaded into the VM in C:\Hackathon. 
* Users should **use** the **Azure Credentials** given to them to login to **Visual Studio**.

# Help and Support

If you require any help during the workshop, please reach out to the instructor / proctors. Instructors / proctors might escalate the issue to remote support team, at that time, please pass on your AAD User ID (aad_user_xyz), so that it is easier to look up your environment.
