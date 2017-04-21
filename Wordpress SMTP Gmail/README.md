# Wordpress SMTP Gmail Plugin

https://wordpress.org/plugins/gmail-smtp/


## Introduction

Sending email via SMTP using Gmail API is one solution to platform with dynamic outgoing IP addresses like Pantheon. This tutorial is a step by step process to enable and configure the gmail-smtp plugin for Wordpress hosted in Pantheon.

## Installation Process

#### 1. At Pantheon Dashboard, switch to [SFTP mode](https://pantheon.io/docs/sftp/) for easy plugin installation.

Once uploaded to DEV, deploy it to TEST and LIVE. You may practice using TEST Environment but you can directly configure LIVE site. Please refer to [Pantheon Workflow]https://pantheon.io/docs/pantheon-workflow how database/files travels between environments.


#### 2. Access the WordPress site. Search and Install the [SMTP Gmail](https://wordpress.org/plugins/gmail-smtp/) plugin. 

![Search and Install SMTP Gmail Plugin](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/1.%20Search%20and%20Install%20SMTP%20Gmail%20Plugin.jpg?raw=true)


#### 3. After Activating the plugin, click Gmail SMTP Plugin Settings.

![Gmail SMTP Plugin Settings](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/2.%20Click%20Settings.jpg?raw=true)


#### 4. From the Basic Setup Instruction, click Web Application that links to creating of project.

![General Settings Page](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/3.%20General%20Settings%20Page.jpg?raw=true)


#### 5. Register your site application for Gmail API starting with creating the project.

![Create a Project](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/4.%20Create%20A%20Project.jpg?raw=true)


#### 6. The Gmail API is enabled and click continue for creating the credentials.

![Go to Credential](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/5.%20Go%20to%20Credentials.jpg?raw=true)


#### 7. Adding the credential to the project by selecting Gmail API and select Web server (e.g. node.js, Tomcat) with User Data and click "What credential do I need"

![Credential Wizzard 1](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/6.%20Credential%20Wizzard%201.jpg?raw=true)


#### 8. Provide the domain URL of the live site and Authorize Redirect URI from No.4 General Setting Page.

![Credential Wizzard 2](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/7.%20Credential%20Wizzard%202.jpg?raw=true)


#### 9. Setup the OAuth2 so the Client ID and Client key will be created.

![Credential Wizzad 3](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/8.%20Credential%20Wizzard%203.jpg?raw=true)


#### 10. Here, take note of the Client ID and download the json file.

![Client ID](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/9.%20Client%20ID.jpg?raw=true)


#### 11. Open the json file with any text editor copy the Client Secret.

![Open downloaded file](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/10.%20Credential%20Wizzard.jpg?raw=true)

![Client Secret](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/11.%20Client%20Secret.jpg?raw=true)


#### 12. Go back to WordPres Gmail Plugin setting page, supply the fields accordingly, and click Save Changes button.

![Saving Credentials](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/12.%20Save%20Credentials.jpg?raw=true)


#### 13. Once changes are saved, a new button will appear below that will ask the application to grant permission.

![Grant Permission](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/13.%20Grant%20Permission.jpg?raw=true)


#### 14. Click Allow to grant permission to your application to read, delete and manage gmail.

![Request Allow Permission](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/14.%20Allow%20Permission.jpg?raw=true)


#### 15. All set, connection button/icon is now in green.

![All Set](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/15.%20All%20Set.jpg?raw=true)


#### 16. Time to test, click Test Email Tab and populate the form for sending a test mail.

![Testing form](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/16.%20Testing%20Form.jpg?raw=true)


#### 17. When the form is submitted, the test mail will provide DEBUG transaction of he emall where you can trace of it's succesfful or not.

![SMTP Transaction Trace](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/17.%20Debug,%20Success.jpg?raw=true)


#### 18. Boom, email received! Have fun!

![Email Received](https://github.com/albertcausing/docs/blob/master/Wordpress%20SMTP%20Gmail/images/18.%20Email%20Recieved.jpg?raw=true)


### Note: Copying the Client ID and Client Secret from this tutorial will not work, as it was already been deleted after the testing.


### Please let us know how it goes on your end. Happy Mailing!


 