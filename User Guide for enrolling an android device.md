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
8.	Enter the email ID & click on **Next**.
9.	Click on **Sign up** under the Sign up for Android Only.
10.	Google Play page will appear, Click on **Getting Started**.
11.	Enter Business name & click on **Next**.
12.	Enter Data Protection Officer & EU representative details.
13.	Click on *I have read and agree to Managed Google Play agreement* & click on **Confirm**.
14.	Set up complete screen appears, click on **Complete Registration**.
15.	Portal will appear with enterprise details.

---

###	To Create Device profile

17.	Go to **Device Profiles & Policies** ➞ **Device Profiles**.
18.	Click on **Create New Profile**.
19.	Click on **Kiosk/Agent option** under Choose Profile Mode.
20.	Enter a profile name and an exit passcode & Click on Submit
21.	In mode for app, Click on **Set as Launcher**.
22.	In Select Apps, enable apps required in the device.
23.	Click on **Create Profile**. 

---

### To Create Device Group

25.	Go to **Groups** ➞ **Device Groups**.
26.	Dropdown CREATE NEW GROUP & Click on **Create New Group**. 
27.	Enter group name & click on Submit.
28.	Create New Device Group screen appears, click on **Next** in Select devices tab.
29.	Under Choose Android Device Profile, select the Profile & click on **Next**.  
30.	Select the profile under any profile tab & click on Next.
31.	Under Add Admin tab, select admin & click on **CREATE DEVICE GROUP**.


### To Create a QR code configuration

33.	Go to **Enrollment Configurations** ➞ **QR Code Configurations**.
34.	Click on **Create Config**. 
35.	Create Device Enrollment Configuration screen will appear.
36.	Under Basic tab enter QR name, Click on **Kiosk/Agent** under Choose Enrollment Type.
37.	Click on **Userless Enrollment** under Choose Enrollment Method.
38.	Enter name convention & click on **Next**. 
39.	Under Group/Profile tab, select Android Device Profile from dropdown & click on **Next**. 
40.	Under Device configuration tab select all options & click on **Next**. 
41.	Under Optional Settings Select additional options like system apps setting, Time zone and data usage.
42.	Click on **Save**. Created QR appears.
43.	  To Enroll device using QR Code
44.	Install the latest app on the device from Google Play Store.
45.	Launch the app.
46.	Click on the **Enroll** & Scan the QR Code generated in previous step.
47.	Proceed to grant all the required permissions to the app.
48.	Complete Setup by setting it up as launcher.

	




