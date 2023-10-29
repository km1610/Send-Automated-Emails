# Send-Automated-Emails
This README will guide you through running the provided Python script for sending emails using the `smtplib` library. It also includes steps to resolve the "username and password not accepted" issue.

### Prerequisites
1. Python installed on your system.
2. A Gmail account for sending emails.
3. A CSV file (`data.csv`) with the email addresses and corresponding message data.
4. A message template file (`message.txt`) for customizing the email content.

### Instructions:

#### 1. Prepare the CSV File and Message Template
- Ensure you have a CSV file named `data.csv` with the recipient's name, email address, and message data.
- Create a message template file named `message.txt` with placeholders for the recipient's name and message content. For example:
  
  ```
  Hello $RECEIVER_NAME,

  This is your message:
  Message 1: $MESSAGE1
  Message 2: $MESSAGE2
  Message 3: $MESSAGE3

  Regards,
  Your Name
  ```

#### 2. Modify Script Variables
- Open the provided script in your favorite text editor.
- Replace the placeholders in the script with your Gmail account details.
  - Replace `'************@gmail.com'` with your Gmail email address.
  - Replace `'**********'` with your Gmail password.

#### 3. Enable Less Secure Apps (Optional)
- To send emails through Gmail using this script, you may need to allow "Less secure apps" in your Gmail settings. However, this is not recommended for security reasons. An alternative is to use an "App Password" or enable 2-Step Verification for added security.

#### 4. Running the Script
- Open a terminal or command prompt.
- Navigate to the directory where the script and data files are located.
- Run the script by executing the following command:
  
  ```bash
  python script_name.py
  ```
  
  Replace `script_name.py` with the name of your script.

#### 5. Resolving "Username and Password Not Accepted" Issue
- If you encounter the "username and password not accepted" issue, it might be due to the security settings in your Gmail account.
- Follow these steps to resolve the issue:
  
  a. Enable "Less secure apps":
     - Go to your Google Account settings.
     - Navigate to the "Security" section.
     - Scroll down and find the "Less secure apps" option.
     - Turn on the "Allow less secure apps" option. This is not recommended for security reasons, but it may resolve the issue.

  b. Use App Password (Recommended):
     - In your Google Account settings, go to the "Security" section.
     - Scroll down to "App Passwords" and generate a new password specifically for this script.
     - Replace your regular Gmail password in the script with the generated app password.

  c. Enable 2-Step Verification (Recommended):
     - Enable 2-Step Verification in your Google Account settings.
     - After enabling 2-Step Verification, generate an "App Password" as described in option b and use it in the script.

#### 6. Run the Script Again
- Once you've resolved the "username and password not accepted" issue using one of the above methods, run the script again as described in step 4.

<hr>

Thank you! ❤️
