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

  *Google Account-> Security-> 2 factor Authentication -> app password -> generate.*

## Step 3: Create a New Email Template
- Click on Email Template and name the template.
- Paste the HTML of the email template. You can use any email template available on GitHub.
- Here we are using a fake Instagram Login page HTML.
  ![go1](https://github.com/user-attachments/assets/c253c88c-53a0-447f-b267-2eb989268097)


## Step 4: Create a Landing Page
- Click on Landing page and name the template.
- Paste the HTML of the landing page (any template available on GitHub).
- Select both Captured Submitted data and passwords.


  ![go9](https://github.com/user-attachments/assets/ea49f0ac-7cab-44ea-8b4a-1bd619a26203)


## Step 5: Launch Phishing Attack
- Click on New Campaign and name the campaign.
- Select Email template and Landing page that you created.
- Select URL from the **ngrok** session that we spawned up, which is the public-facing IP.
- Select the launch date and group and click on launch.

Now that the campaign is launched, you can start analysing the simulated attack.

## Step 6: Analysing the attack

- Review the data collected from the phishing campaign.
- Identify which users fell for the phishing attack and analyze the captured credentials. 

Expected Output: A detailed report on the effectiveness of the phishing campaign, highlighting potential security weaknesses.
![go2](https://github.com/user-attachments/assets/efece53b-019e-4869-9312-7a3a3649bd17)

![go3](https://github.com/user-attachments/assets/33b4a27e-6faa-4448-a930-8bcfc260a23c)

![go4](https://github.com/user-attachments/assets/79f036a6-fde4-4755-96b2-ab9ea6971d82)



## Defending against the attack
- Educating the users and employees not to click on any suspicious links or attachments.
- To immediately report such emails to the concerned team.
- Enabling filtering to block phishing emails.
- Multi-factor authentication system.
- Updating and securing the systems.
- Develop a phishing awareness training program for employees and track the progress.


  

  

