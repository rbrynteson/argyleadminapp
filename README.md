## Argyle Admin App (AAA)
Welcome to the Argyle Admin App!  This application is based on a series of samples projects and open source components to create an admin tool for Microsoft Teams.  This is 100% hosted and available in GitHub.  Feel free to contribute.

## Getting Started
Using the app requires a few things to be setup.

1. Configure an Azure Application.  Go to the [Azure Portal](https://portal.azure.com), Azure Active Directory, App Registrations and choose New Registration.
![alt text](https://theargylemvp.com/assets/images/5-23-2019-1.png "")
2. Enter a Name, choose "accounts in this organization only" and enter https://app.theargylemvp.com as the return URL.
![alt text](https://theargylemvp.com/assets/images/5-23-2019-2.png "")
3. Once created, go to API Permissions and assign the permissions as needed.
* ChannelMessage.Read.All (Application)
* Group.Read.All (Application)
* Group.Read.All (Delegated)
* User.Read (Delegated)
![alt text](https://theargylemvp.com/assets/images/5-23-2019-3.png "")
4. On the Overview page, note your Client ID and Tenant ID. 
![alt text](https://theargylemvp.com/assets/images/5-23-2019-4.png "")

Once you have this data and have your app setup.  Head over to [https://app.theargylemvp.com ](https://app.theargylemvp.com ) and use one of your organizations logins to get the information.

## Another Option
Want to run on your own server?

1. Go to github [https://github.com/rbrynteson/theargylemvp](https://github.com/rbrynteson/theargylemvp) and Clone/Download the application.
2. Install Node [https://nodejs.org/en/](https://nodejs.org/en/).
3. Go to the folder you just cloned/downloaded.
4. Configure your server.
* npm install express
* npm install morgan
* node server.js

The server will run on the port defined, [http://localhost:30662](http://localhost:30662).  Important, make sure to update your Return URL to include this URL.  

## Useful Links
1. [Getting Started](https://aka.ms/aadv2)
2. [Code Samples](https://github.com/azure-samples/)

## The License
Licensed under the MIT License (the "License");
