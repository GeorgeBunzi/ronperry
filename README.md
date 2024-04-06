# Instruction Files for Ron Perry #

## Tables of Contents
### I. WordPress
### II. Images
### III. Fonts
### IV. Emails
### V. FTP

---

## I. WordPress

## II. Images

## III. Fonts

## IV. Emails

## V. FTP

** Install FileZilla ** (client version only)

https://filezilla-project.org/

Set up the domain to be hosted on DreamHost (make it a live website, all domains must have a site before it can be viewed publicly)
- Log onto dreamhost.com
- Click on Websites (on the left menu)
- Click on Manage Websites (all the websites will display on the right - if the domain has a globe, then it is just a domain and not yet set up to be a site)
- Locate the domain (to be set up as a website)
- Click on Manage button associated with that domain (a page will display)
- Click Add Hosting button (this tells DreamHost to create a website for this domain - NOTE: The website will be created as an unsecured site as http://)
- Wait until DreamHost is done setting up the website (may take a while)

Request an SSL certificate (to use https:// - NOTE:  SSL certificate can only be requested on websites not registered domains)
- Log onto dreamhost.com
- Click on Websites (on the left menu)
- Click on Manage Websites (all the websites will display on the right)
- Locate the desired website (with an open lock icon)
- Click on the vertical ellipses to the far right of this domain (a popup menu will display)
- Click on SSL Security (the SSL page will display)
- Select the Let's Encrypt Certificate option (a request for the SSL certificate will be sent to DreamHost)
- Wait for DreamHost to generate the certificate (may take a while)
- Click on Websites (on the left menu) later to refresh the page (if DreamHost is done creating the Let's Encrypt Certificate, then the domain will have a closed lock icon)

Create an FTP account on DreamHost
- Log onto dreamhost.com
- Click on Websites (on the left menu)
- Click on SFTP Users & Accounts (SFTP - Secure File Transfer Protocol)
- Click on Create User button (blue button on the top right)
- Enter a user name (must be unique)
- Select a server (to assign the account to a location defined for the domain, each FTP user can only be assigned to a location)
- Enter a password (at least 8 characters, no "123" anywhere)
- Click Create User button
- If the information is valid, DreamHost will create the account (it may take a few minutes)
- Once done, the account will show up on the page

Set up FileZilla to access the DreamHost server (where site contents reside)
- Run FileZilla
- Maximize the screen (to have a better view)
- Click on File
- Click on Site Manager (a dialog will pop up showing all the FTP sites that have been set up previously)
- Click on New Site button (at the bottom of the dialog)
- Enter a name for the new FTP site (usually the domain name)
- Click on the Protocol dropdown box on the right
- Select SFTP - SSH File Transfer Protocol
- Enter the FTP host name
- Enter 22 the port
- Leave Logon Type as Normal
- Enter the FTP user name for User
- Enter the password for Password
- Click Ok button (the new FTP site will be added to the left panel)

Connect to the DreamHost server
