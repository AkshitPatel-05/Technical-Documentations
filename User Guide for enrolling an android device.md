### Introduction

This guide shows step by step instructions to enroll an android device using Userless kiosk with the help of QR code. The guide will be useful when a single device is shared by multiple users. This process is useful for IT admins to remotely configure the devices.

---
### Prerequisites
Before starting, make sure the following:
•	Active admin account.
•	An Android device that supports QR code enrollment (Android 7.0+ recommended).
•	Stable internet connection on both admin PC and device.

### Step-by-Step Instructions

1.	Log in to your **Dashboard**.
2.	Go to **Getting Started** > **Android Enterprise Setup**.
3.	Dropdown **Google Android Enterprise** with Device Manager.
4.	Click on **Register with Any Email**. 
5.	Screen to provide email ID will appear.
6.	To Set up Android Enterprise using a non-corporate/personal Gmail ID
7.	Enter the email ID & click on **Next**.
8.	Click on **Sign up** under the Sign up for Android Only.
9.	Google Play page will appear, Click on **Getting Started**.
10.	Enter Business name & click on **Next**.
11.	Enter Data Protection Officer & EU representative details.
12.	Click on *I have read and agree to Managed Google Play agreement* & click on **Confirm**.
13.	Set up complete screen appears, click on **Complete Registration**.
14.	Portal will appear with enterprise details.

---

###	To Create Device profile

1.	Go to **Device Profiles & Policies** ➞ **Device Profiles**.
2.	Click on **Create New Profile**.
3.	Click on **Kiosk/Agent option** under Choose Profile Mode.
4.	Enter a profile name and an exit passcode & Click on Submit
5.	In mode for app, Click on **Set as Launcher**.
6.	In Select Apps, enable apps required in the device.
7.	Click on **Create Profile**. 

---

### To Create Device Group

1.	Go to **Groups** ➞ **Device Groups**.
2.	Dropdown CREATE NEW GROUP & Click on **Create New Group**. 
3.	Enter group name & click on Submit.
4.	Create New Device Group screen appears, click on **Next** in Select devices tab.
5.	Under Choose Android Device Profile, select the Profile & click on **Next**.  
6.	Select the profile under any profile tab & click on Next.
7.	Under Add Admin tab, select admin & click on **CREATE DEVICE GROUP**.


### To Create a QR code configuration

1.	Go to **Enrollment Configurations** ➞ **QR Code Configurations**.
2.	Click on **Create Config**. 
3.	Create Device Enrollment Configuration screen will appear.
4.	Under Basic tab enter QR name, Click on **Kiosk/Agent** under Choose Enrollment Type.
5.	Click on **Userless Enrollment** under Choose Enrollment Method.
6.	Enter name convention & click on **Next**. 
7.	Under Group/Profile tab, select Android Device Profile from dropdown & click on **Next**. 
8.	Under Device configuration tab select all options & click on **Next**. 
9.	Under Optional Settings Select additional options like system apps setting, Time zone and data usage.
10.	Click on **Save**. Created QR appears.
11.	  To Enroll device using QR Code
12.	Install the latest app on the device from Google Play Store.
13.	Launch the app.
14.	Click on the **Enroll** & Scan the QR Code generated in previous step.
15.	Proceed to grant all the required permissions to the app.
16.	Complete Setup by setting it up as launcher.

	




