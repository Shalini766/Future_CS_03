# Creating a Phishing Attack using Gophish
## Objective
This project is based on building and simulating a phishing attack by creating a fake Instagram alert. Phishing is a common type of cyber attack often used to steal credentials like passwords, data, and other confidential information by tricking users.
## Tools Used
**Gophish**- Open source phishing tool.

**Email Account**- To send phishing emails.

**ngrok**- Creates a secure tunnel between local web servers and a public ngrok endpoint by assigning a public IP to test the applications and deploying them.

This project is done on **Windows OS**. One can also use **Kali Linux** to build this project.

## Installation of Gophish and ngrok
**Gophish**
- Download from the official website https://getgophish.com.
- Extract the files and click on the gophish.exe file.
- The command prompt appears where there will be a username and a password.
- Access the gophish on https://localhost:3333
- 
**ngrok**
- Download the latest version from https://ngrok.com
- Extract and run the ngrok.exe file
- Go to the ngrok and copy the authentication token
- Run the command in the prompt, i.e., ngrok config add-authtoken <token >
- You get the public-facing IP where you can host your webpage on http://localhost:80

## Steps

## Step 1: Create users and groups.
- Create a new user group with the target email addresses.
  
## Step 2: Set up a Sending Profile
- Open the Gophish web interface at https://localhost:333
- Specify the Name, SMTP, Host, Username, and Password on the Sending Profile.

   For the password, you need to use an app password. This can be generated in your Google account.

  Google Account-> Security-> 2 factor Authentication -> app password -> generate.

## Step 3: Create a New Email Template
- Click on Email Template and name the template.
- Paste the HTML of the email template. You can use any email template available on GitHub.
- Here we are using a fake Instagram Login page HTML.

## Step 4: Create a Landing Page
- Click on Landing page and name the template.
- Paste the HTML of the landing page (any template available on GitHub).
- Select both Captured Submitted data and passwords.


  

  

