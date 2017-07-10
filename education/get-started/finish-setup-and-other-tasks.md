---
title: Finish Windows 10 device setup and other tasks
description: Learn how to use the new Microsoft Education system to set up a cloud infrastructure for your school, acquire devices and apps, and configure and deploy policies to your Windows 10 devices.
keywords: education, Microsoft Education, full cloud IT solution, school, deploy, setup, manage, Windows 10, Intune for Education, Office 365 for Education, School Data Sync, Microsoft Teams, Microsoft Store for Education, Azure AD, Set up School PCs
ms.prod: w10
ms.mktglfcycl: deploy
ms.sitesec: library
ms.topic: get-started
localizationpriority: high
ms.pagetype: edu
author: CelesteDG
ms.author: celested
ms.date: 07/10/2017
---

# Finish Windows 10 device setup and other tasks
Once you've set up your Windows 10 education device, it's worth checking to verify the following:

> [!div class="checklist"]
> * Correct device setup
> * Device is Azure AD joined

You can watch the video to see how this is done, or follow the step-by-step guide. </br>

<div style="position:relative;height:0;padding-bottom:56.25%"><iframe src="https://www.youtube.com/embed/nhQ_4okWFmk?ecver=2" width="640" height="360" frameborder="0" style="position:absolute;width:100%;height:100%;left:0" allowfullscreen></iframe></div>

You can watch the descriptive audio version here: [Microsoft Education: Verify Windows 10 education devices are Azure AD joined and managed (DA)](https://www.youtube.com/watch?v=_hVIxaEsu2Y)

## Verify correct device setup
Verify that the device is set up correctly and boots without any issues.

**Verify that the device was set up correctly**
1. Confirm that the Start menu contains a simple configuration.
2. Confirm that the Store and built-in apps are installed and working. The apps pushed down from Intune for Education will appear under **Recently added**. 

  > [!NOTE]  
  > It may take some time before some apps are pushed down to your device from Intune for Education. Check again later if you don't see some of the apps you provisioned for the user.

  **Figure 1** - Sample list of apps for a user

  ![Apps list contains the apps provisioned for the user](images/win10_start_checkapps.png)

## Verify the device is Azure AD joined
Let's now verify that the device is joined to your organization's Azure AD and shows up as being managed in Microsoft Intune for Education.

**Verify if the device is joined to Azure AD**
1. Log in to the <a href="https://intuneeducation.portal.azure.com/" target="_blank">Intune for Education console</a>.
2. Select **Groups** and select **All Devices**.
3. In the **All Devices** page, see the list of devices and verify that the device you're signed into appears on the list.

  **Figure 2** - List of all managed devices

  ![Verify that the device is managed in Intune for Education](images/i4e_groups_alldevices_listofaadjdevices.png)

4. On the Windows 10 education device, click **Start** and go to **Settings**. 
5. Select **Accounts > Access work or school**.
6. In the **Access work or school** page, confirm that the device is connected to the organization's Azure AD.

  **Figure 3** - Confirm that the Windows 10 device is joined to Azure AD

  ![Confirm that the Windows 10 device is joined to Azure AD](images/win10_confirmaadj.png)

**That's it! You're done!** You've completed basic cloud setup, deployment, and management using Microsoft Education. 

You can follow the rest of the walkthrough to finish setup and complete other tasks, such as:

> [!div class="checklist"]
> * Update group settings in Intune for Education
> * Configure Azure settings
> * Complete Office 365 for Education setup
> * Add more users
> * Connect other devices, like BYOD devices, to your cloud infrastructure

You can watch the following video to see how to update group settings in Intune for Education and configure Azure settings. Or, you can follow the step-by-step guide for these tasks and the other tasks listed above.

<div style="position:relative;height:0;padding-bottom:56.25%"><iframe src="https://www.youtube.com/embed/M6-k73dZOfw?ecver=2" width="640" height="360" frameborder="0" style="position:absolute;width:100%;height:100%;left:0" allowfullscreen></iframe></div>

You can watch the descriptive audio version here: [Microsoft Education: Update settings, apps, and Azure AD settings for your education tenant (DA)](https://www.youtube.com/watch?v=-Rz3VcDXbzs)

## Update group settings in Intune for Education
If you need to make changes or updates to any of the apps or settings for the group(s), follow these steps.

1. Log in to the <a href="https://intuneeducation.portal.azure.com/" target="_blank">Intune for Education console</a>.
2. Click **Groups** and then choose **Settings** in the taskbar at the top of the page.
3. You will see the same settings groups that you saw in express setup for Intune for Education as well as other settings categories such as **Windows Defender settings**, **Device sharing**, **Edition upgrade**, and so on.

  **Figure 4** - See the list of available settings in Intune for Education

  ![See the list of available settings in Intune for Education](images/i4e_groups_settingslist_full.png)

4. Keep the default settings or configure the settings according to your school's policies. 

  For example, you can configure the diagnostic data sent to Microsoft in **Basic device settings > Send diagnostic data**. 

5. Click **Save** or **Discard changes**.

## Configure Azure settings
After completing the basic setup for your cloud infrastructure and confirming that it is up and running, it's time to prepare for additional devices to be added and enable capabilities for the user to use.

### Enable many devices to be added by a single person 
When a device is owned by the school, you may need to have a single persion adding many devices to your cloud infrastructure. 

Follow the steps in this section to enable a single person to add many devices to your cloud infrastructure.

1. Sign in to the <a href="https://portal.office.com" target="_blank">Office 365 admin center</a>.
2. Configure the device settings for the school's Active Directory. To do this, go to the new Azure portal, <a href="https://portal.azure.com" target="_blank">https://portal.azure.com</a>.
3. Select **Azure Active Directory > Users and groups > Device settings**.

  **Figure 5** - Device settings in the new Azure portal

  ![Configure device settings in the new Azure portal](images/azure_newportal_usersandgroups_devicesettings.png)

4. Find the setting **Maximum number of devices per user** and change the value to **Unlimited**.
5. Click **Save** to update device settings.

### Enable roaming settings for users
When students move from using one device to another, they may need to have their settings roam with them and be made available on other devices. 

Follow the steps in this section to ensure that settings for the each user follow them when they move from one device to another.

1. Sign in to the <a href="https://portal.office.com" target="_blank">Office 365 admin center</a>.
3. Go to the new Azure portal, <a href="https://portal.azure.com" target="_blank">https://portal.azure.com</a>.
3. Select **Azure Active Directory > Users and groups > Device settings**.
4. Find the setting **Users may sync settings and enterprise app data** and change the value to **All**.

  **Figure 6** - Enable settings to roam with users

  ![Enable settings to roam with users](images/azure_usersandgroups_devicesettings_ers.png)

5. Click **Save** to update device settings.

## Complete Office 365 for Education setup
Now that your basic cloud infrastructure is up and running, it's time to complete the rest of the Office 365 for Education setup. You can find detailed information about completing Office 365 setup, services and applications, troubleshooting, and more by reading the <a href="https://support.office.com/en-US/Article/set-up-Office-365-for-business-6a3a29a0-e616-4713-99d1-15eda62d04fa#ID0EAAAABAAA=Education" target="_blank">Office 365 admin documentation</a>.

## Add more users
After your cloud infrastructure is set up and you have a device management strategy in place, you may need to add more users and you want the same policies to apply to these users. You can add new users to your tenant simply by adding them to the Office 365 groups. Adding new users to Office 365 groups automatically adds them to the corresponding groups in Intune for Education.

See <a href="https://support.office.com/en-us/article/Add-users-to-Office-365-for-business-435ccec3-09dd-4587-9ebd-2f3cad6bc2bc" target="_blank">Add users to Office 365</a> to learn more. Once you're done adding new users, go to the <a href="https://intuneeducation.portal.azure.com/" target="_blank">Intune for Education console</a> and verify that the same users were added to the Intune for Education groups as well.

## Connect other devices to your cloud infrastructure
Adding a new device to your cloud-based tenant is easy. For new devices, you can follow the steps in [6. Set up Windows 10 devices](#6-set-up-windows-10-devices). For other devices, such as those personally-owned by teachers who need to connect to the school network to access work or school resources (BYOD), you can follow the steps in this section to get these devices connected.

  > [!NOTE]  
  > These steps enable users to get access to the organization's resources, but it also gives the organization some control over the device.

**To connect a personal device to your work or school**

1. On your Windows device, go to **Settings > Accounts**.
2. Select **Access work or school** and then click **Connect** in the **Connect to work or school** page.
3. In the **Set up a work or school account** window, enter the user's account info.

  For example, if a teacher connects their personal device to the school network, they'll see the following screen after typing in their account information.

  **Figure 7** - Device is now managed by Intune for Education

  ![Device is managed by Intune for Education](images/byob_aad_enrollment_intune.png)

4. Enter the account password and then click **Sign in** to authenticate the user.

   Depending on the organization's policy, the user may be asked to update the password.

5. After the user's credentails are validated, the window will refresh and will now include an entry that shows the device is now connected to the organization's MDM. This means the device is now enrolled in Intune for Education MDM and the account should have access to the organization's resources.

  **Figure 8** - Device is connected to organization's MDM

  ![Device is connected to organization's MDM](images/win10_connectedtoorgmdm.png)

6. You can confirm that the new device and user are showing up as Intune for Education-managed by going to the Intune for Education management portal and following the steps in [6.3 Verify the device is Azure AD joined](#63-verify-the-device-is-azure-ad-joined). 

  It may take several minutes before the new device shows up so check again later.

  
## Related topic
[Get started: Deploy and manage a full cloud IT solution with Microsoft Education](get-started-with-microsoft-education.md)