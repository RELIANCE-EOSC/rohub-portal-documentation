---
layout: default
title: ROHub authentication
nav_order: 2
permalink: /docs/ROHub-authentication
---

# ROHub authentication
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
------------

## Login Section
The login (Sign in/Sign up) is available on the menu bar of the homepage. The keycloak authentication system allows the users to login either with existing EGI credentials or users can register themselves with their own login and password. Once registered the authentication system allows the registered users to sign in to the ROhub portal. The sections below briefly describe the login and sign up functionalities of the ROhub portal.

### Signing into the ROHub Account
On clicking any of the "Sign in '' or "Sign up" the user is navigated to the authentication page. From here the user can sign in either through the EGI Check-in on clicking the "Login with EGI Check-in". On clicking the user is redirected to the EGI authentication system and on completion the user gets signed into the ROHub Portal via the EGI check in process. The user can also sign in from this page with his registered credentials for ROHUb portal.


<p align="center"> <img src="https://box.psnc.pl/f/97505de421/?raw=1" width="500"> </p>
<div align="center"> Figure 1: Login page in ROHub portal </div>


### Password Reset
The authentication page also allows the user to go for a resetting of password. Once the user clicks on the “Forgot password?”, he gets redirected to the page where the user can provide the email address and the instructions on how to create a new password will be sent as an email. After providing the email address and clicking “Submit” the user gets an email. The user can navigate back to the login page by clicking “Back to Login”.

<p align="center"> <img src="https://box.psnc.pl/f/4e010afa88/?raw=1" width="500"> </p>
<div align="center"> Figure 2: Password Reset form </div>

### Registering the new User
New users can be registered into the ROhub portal from the login page. Once the new user clicks “Register” the registration form opens. In the various fields of the form the user can provide registration details (e.g. first name, last name, email, and password). The registration procedure completes on clicking the “Register” at the end of the form and “Back to Login” navigates the user back to the login page.

<p align="center"> <img src="https://box.psnc.pl/f/ef8a6b0b57/?raw=1" width="500"> </p>
<div align="center"> Figure 3: User registration in ROHub </div>


## Account Settings
After successfully logging in to the ROHUb portal, a user can access his “Account settings”  from the right side corner of the ROHub landing page. After clicking the drop down arrow beside the authentication section the user can see “Account settings” and “Log Out”. On clicking the Account settings the user gets navigated to various sections. In the account settings the user can access various forms and edit them  present in each section listed on the left hand side of the page. The various sections of the account settings are described below. On the top right hand side of the page there are options to change the language (English and Polish as of now). “Back to reliance.rohub.org” takes the user back to the homepage of the ROHub portal and “Sign Out” logs the user out and takes back to the login page.

<p align="center"> <img src="https://box.psnc.pl/f/89815b5247/?raw=1" width="800"> </p>
<div align="center"> Figure 4: Account settings in ROHub </div>

### Account
Once into the account settings navigation pages, the user can access the “Edit Account” form from the first “Account” section present on the list of sections on the left hand side of the account settings homepage. In the “Edit Account” form the user can update the user information in various fields provided such as “Email”, “Salutation”, “First name”, “Last name”, “Affiliation”, “Description”, “Area of interest”, “B2SHARE token”, “zenodo token”, “ORCID”, "Resources Storage" (Deafault or B2DROP), "B2DROP Username", "B2DROP Password" and "ADAM Platform Key". Out of all this information the required fields are marked with a red dot. On completion the user can click on “Save” to complete the update of the Account information.


<p align="center"> <img src="https://box.psnc.pl/f/9d9e6ab27d/?raw=1" width="700"> </p>
<div align="center"> Figure 5: Edit User Account in ROHub </div>

### Password
From the “Password” section the user can change the existing password with a new one. From the account settings the user doesn't need to provide an email address. On clicking “Save” completes the password change.

<p align="center"> <img src="https://box.psnc.pl/f/e0b22fa99c/?raw=1" width="500"> </p>
<div align="center"> Figure 6: Changing Password via account settings </div>


### Authenticator
This section allows the user to have a second level authentication. This is done through third party authentication applications (e.g. FreeOTP, Google Authenticator). The applications scan the QR code provided in the user’s account and generate an One Time Password (OTP) to authenticate the user. This OTP along with the name of the users’ device can be saved in the user account settings of the ROHub from this section. If the user has a problem scanning the QR code, on clicking the “Unable to scan?” the user gets navigated to another similar page, where a 32 digit key appears along with some instructions for the user specific to the above mentioned third party applications. The user can alternatively use this 32 digit key to generate the OTP. Clicking “Scan barcode” brings the user back to the page of the QR code if he wishes to do so. The user can finally provide the OTP and an optional device name in the respective fields and click on “Save” to complete the whole process.

<p align="center"> <img src="https://box.psnc.pl/f/4382c952a1/?raw=1" width="500"> </p>
<div align="center"> Figure 7: Third party authentication in ROHub </div>

### Federated identity
This section shows the user identity in EGI check-in, if any, which is essentially the username of the user in the EGI system. The user can add/remove the identity on clicking the “+”/“-” icon alongside the box showing the federated identity. If the user is logged in on clicking the “+” icon the username of the EGI is added in the federated identity.

<p align="center"> <img src="https://box.psnc.pl/f/5c7504546a/?raw=1" width="500"> </p>
<div align="center"> Figure 8: Federated identity in ROHub </div>

### Sessions
In this section the current session for the user account is shown. The session record consists of information like the user IP address, session start date and time, session end date and time, the date and time of the last access by the user and the name of the clients logged in. On clicking “Log out all sessions” the user gets logged out from the displayed session in this section.

<p align="center"> <img src="https://box.psnc.pl/f/465d2ce838/?raw=1" width="700"> </p>
<div align="center"> Figure 9: User session in ROHub portal </div>

### Applications
This section shows the user a table that contains the name of  the applications and his available roles from the logged in account. The user can see the granted permission for him in the table. Some of the applications can be accessed from this list of the applications in the table on clicking the link provided.

<p align="center"> <img src="https://box.psnc.pl/f/31390bee06/?raw=1" width="700"> </p>
<div align="center"> Figure 10: Applications in Account Settings </div>

### Log
The log section holds all the records of all available actions from the user side. The log table contains the “Date”, name of the “Event”, “IP” of the user and name of the used “Client”. In the “Details” the description of the action is provided.

<p align="center"> <img src="https://box.psnc.pl/f/36892a7123/?raw=1" width="700"> </p>
<div align="center"> Figure 11: Account Logs in ROHub </div>
