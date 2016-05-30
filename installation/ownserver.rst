Installation - Using your own web server
================================================

SDonate also comes with all of the files necessary for you to set up a store on your own web server. Follow the instructions below carefully to avoid any errors.

Requirements
------------------------
Before installing SDonate, you should check that your web server has the following requirements for SDonate to work.

*PHP >= 5.5
*MySQL
*PDO

SDonate also requires access to some functions that some hosts may block. To check these functions work, download https://sdonate.com/downloads/compatibilitychecker.zip then unzip it into the root folder of your web host (usually called "public_html" or "public"), then go to http://<yourdomain.tld>/compatibilitychecker.php (for example, if your domain is "myamazingdomain.com", go to http://myamazingdomain.com/compatibilitychecker.php). If everything is alright, it will say your host is compatible, otherwise you will need to contact your host to fix any issues or find a new host.

1. Extracting SDonate
---------------------------
The first thing you will need to do after do after downloading SDonate is extract the zip. It's best to extract it into a folder on your desktop for easy access.

2. Setting the admin
--------------------------------
After you've extracted SDonate, go into the "web" folder and open the file called "install.php" using a text editor. Notepad will work but a better text editor such as Notepad++ is preferable as it makes things easier to see. Once you've opened it, you will see three lines starting with $adminsteamid, $adminusername and $adminpassword. You will need to decide whether you want the first admin (you) to log in using a username and password or using Steam login. If you want to log in using Steam, edit the line starting with $adminsteamid and put your Steam ID in between the quotation marks. For example, my Steam ID is 76561198134262586, so I would change it to: ::

    $adminsteamid = '76561198134262586';

If you want to use a username and password to log in as admin, make sure that $admingsteamid is empty, so it looks like: ::

    $adminsteamid = '';

Then edit $adminusername and $adminpassword with the username and password you want. For example, if my username is "adminuser" and my password is "mypassword1", I would change it to: ::

    $adminusername = 'adminuser';

    $adminpassword = 'mypassword1';

.. note::
    SDonate requires $adminsteamid to be in SteamID64 format and NOT SteamID32. A SteamID64 looks like '76561198134262586' while a SteamID32 looks like 'STEAM_0:0:86998429'.

3. Setting up the MySQL database
-------------------------------------------
