⬅️ [Previous: SIEM Wazuh Installation](04-siem-wazuh-installation.md) | [Next: Osticket and Wazuh Integration ➡️](06-osticket-wazuh-integration.md)

# Step 3: ⚙️ Osticket Installation and Configuration

### Step 3.1: Installing LAMP stack
![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation1.png)
- Installed the Apache, MySQL, and PHP in a Linux Ubuntu Server (LAMP stack).

![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation2.png)
- Verified the LAMP stack if successfully installed.
---
### Step 3.2: Configuring MySQL Database and installing Osticket
![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation3.png)
- Configure MySQL using the command **sudo mysql_secure_installation** to improve security of the database.

![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation4.png)
- Created a database and a user for Osticket.
- Installed Osticket using the wget command to fetch the packages from the github.

![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation5.png)
- Verified Osticket if successfully installed.
- Used **sudo unzip /tmp/osTicket-v1.18.1.zip -d /tmp/osticket** to extract the file to a new folder.
- Created a new directory using **sudo mkdir /var/www/html/osticket/** where os ticket will permanently live on the server.
- Used the command **sudo cp -r /tmp/osticket/upload/* /var/www/html/osticket/** to copy all of the osticket application file from the temporary download location into a permanent folder.
- Used the command **sudo chown -R www-data:www-data /var/www/html/osticket** to change the ownership of all osTicket files to a user called **www-data**.

![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation6.png)
- Open the Osticket in a browser to check if the Osticket is working.

![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation7.png)
- Configured and Filled up the information needed for the osticket to work including the osticket admin credentials.
---
### Step 3.3: Validation Step: Verified Osticket installation completed
![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation8.png)
- Successfully installed osticket in the Ubuntu Server.

![Screenshot](../screenshots/Osticket-Setup-Installation/OsticketInstallation9.png)
- This image shows the dashboard of the Osticket for the Users.
- The directory **http://192.168.1.50/scp** is used to logged-in as an admin user.
---

⬅️ [Previous: SIEM Wazuh Installation](04-siem-wazuh-installation.md) | [Next: Osticket and Wazuh Integration ➡️](06-osticket-wazuh-integration.md)
