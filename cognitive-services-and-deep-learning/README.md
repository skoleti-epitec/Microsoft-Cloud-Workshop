# Introduction

# Sign-up for Workshop Environment

To make it easier for you to work on the labs, you are provided with pre-provisioned Azure environment. You will receive sign-up link for the lab environment from your instructor. 

* Register for the lab environment by providing your information and clicking on **Submit** button.

* On the next page, click the **Launch Lab** button.
 
* Wait for the lab environment to be provisioned. Sometimes this can take upto **10 minutes**. Once environment provisioning is complete, you will receive details in email as well as in the browser.
 
 > Note: Lab environment is enabled only for specific duration or workshop end time - whichever is earlier. At the end of the allowed time, environment will be self-destructed. Also, for multi-day workshops, all virtual machines will be shutdown at 7 PM local time and start at 8AM local time.

# Verify the pre-provisioned Environment

## Verify Azure Access

Open a browser instance in private or incognito mode and login to [Microsoft Azure Portal](https://portal.azure.com) using the credentials provided.

> Note: You might have an existing Azure Credential. For the pre-provisioned environment, new Microsoft Azure environment is provisioned and new AAD user is created for you. To prevent conflict with your existing accounts, it is advised to use In Private mode of IE / IE Edge or Incognito mode of Chrome browser.

## Verify Pre-requisite Azure Resources

You are provided a Data Science Virtual Machine - Windows 2016 with additional softwares configured in advance. FQDN of the virtual machine and administrator credentials are provided in the lab details page.You can remote into the virutal machine using the provided credentials. Please use this VM during the lab instead of create new VM as specified in Task-1.


# Known Issues
* In **Exercise 1**, Task 1 -> Step 3 search for **Machine Learning Experimentation** and select **Machine Learning Experimentation (Retiring)** from the list that appears because **Machine Learning Experimentation (preview)** is updated with **Machine Learning Experimentation (Retiring)** in Azure Portal.

* In **Exercise 2**, task 1 you need to edit the command for creating the cluster environment to specify using existing resource group which is pre-created for you, otherwise the deployment would fail. Make a note of name of your existing resource group and include in the command as specified below
```
az ml env setup -c -g <resource group> -n mcwailabenv --location eastus2
```

### Connecting DSVM with RDP having issue addresses CredSSP

> **Possible Solutions**:

* With the release of the March 2018 Security bulletin, there was a fix that addressed a CredSSP, “Remote Code Execution” vulnerability (CVE-2018-0886) which could impact RDP connections. 
**Resolution**
Please follow the instruction under https://github.com/SpektraSystems/Microsoft-Cloud-Workshop/blob/master/RDP%20CredSSP/README.md

# Notes to Instructors / Proctors

* LABVM is already deployed in ODL_csdl-XXXXX Resource Group and configured with all the requirements.
* Installation of AzureML Workbench Setup will take around 30-45 minutes to install.

# Help and Support

If you require any help during the workshop, please reach out to the instructor / proctors. Instructors / proctors might escalate the issue to remote support team, at that time, please pass on your AAD User ID (aad_user_xyz), so that it is easier to look up your environment.



