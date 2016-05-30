Installation - Using your own web server
================================================

.. warning::
    Before following the instructions here make sure you have completed the instructions in :doc:`apikey`.

SDonate comes with all of the files necessary for you to set up a store on your own web server. Follow the instructions below carefully to avoid any errors.

Requirements
------------------------
Before installing SDonate, you should check that your web server has the following requirements for SDonate to work.

* PHP >= 5.5
* MySQL
* PDO

SDonate also requires access to some functions that some hosts may block. To check these functions work, download https://sdonate.com/downloads/compatibilitychecker.zip then unzip it into the root folder of your web host (usually called "public_html" or "public"), then go to http://<yourdomain.tld>/compatibilitychecker.php (for example, if your domain is "myamazingdomain.com", go to http://myamazingdomain.com/compatibilitychecker.php). If everything is alright, it will say your host is compatible, otherwise you will need to contact your host to fix any issues or find a new host.

1. Extracting SDonate
---------------------------
The first thing you will need to do after do after downloading SDonate is extract the zip. It's best to extract it into a folder on your desktop for easy access.

2. Setting the admin
--------------------------------
After you've extracted SDonate, go into the "web" folder and open the file called "install.php" using a text editor. Notepad will work but a better text editor such as Notepad++ is preferable as it makes things easier to see. Once you've opened it, you will see three lines starting with ``$adminsteamid``, ``$adminusername`` and ``$adminpassword``. You will need to decide whether you want the first admin (you) to log in using a username and password or using Steam login. If you want to log in using Steam, edit the line starting with ``$adminsteamid`` and put your Steam ID in between the quotation marks. For example, my Steam ID is 76561198134262586, so I would change it to: ::

    $adminsteamid = '76561198134262586';

If you want to use a username and password to log in as admin, make sure that $admingsteamid is empty, so it looks like: ::

    $adminsteamid = '';

Then edit $adminusername and $adminpassword with the username and password you want. For example, if my username is "adminuser" and my password is "mypassword1", I would change it to: ::

    $adminusername = 'adminuser';

    $adminpassword = 'mypassword1';

.. note::
    SDonate requires ``$adminsteamid`` to be in SteamID64 format and NOT SteamID32. A SteamID64 looks like '76561198134262586' while a SteamID32 looks like 'STEAM_0:0:86998429'.

3. Setting your API keys
-----------------------------------------
In the extracted SDonate folder, open the "web" folder again then open "config.php". You will see a line starting with ``$sdonateapi``, inside the quotation marks next to this copy your SDonate API key you generated earlier. You will also need your Steam API key. To get your Steam API key head over to https://steamcommunity.com/dev/apikey. If you have not already filled in this form, do so now to get your Steam API Key. Now, in "config.php", in the quotation marks next to ``$steamapi`` copy your Steam API key and save your changes.

4. Setting up the MySQL database
-------------------------------------------
Using a database manager like phpMyAdmin or your host's own database management system, you will need to create a database for SDonate as well as a user that has full access to that database, the instructions for this vary by system so they are not covered here, but it should be simple enough. In "config.php", you will see four lines starting with ``$dbhost``, ``$dbname``, $dbusername`` and ``$dbpassword``. ``$dbhost`` is the ip of your MySQL server. Unless your MySQL server is on a different IP to your website, you should leave this as 'localhost'. In the quotation marks next to ``$dbname`` enter the name of the database you created, this should include any prefixes also. Next to ``$dbusername`` and ``$dbpassword`` enter your database user's username and password, then save your changes.

5. Setting the main currency of your store
--------------------------------------------------
In "config.php", next to ``$currencycode`` you will need to enter the currency code of the main currency you want your store to use. Users will be able to pay using their own currencies, but this is the currency that all of your prices will be displayed in. Below is a list of valid currency codes. You only need to enter the three letter code.

* **AUD** - Australian Dollar
* **CAD** - Canadian Dollar
* **DKK** - Danish Krone
* **EUR** - Euro
* **GBP** - British Pound Sterling
* **MXN** - Mexican Peso
* **NOK** - Norwegian Krone
* **NZD** - New Zealand Dollar
* **PLN** - Polish Zloty
* **NOK** - Norwegian Krone
* **RUB** - Russian Ruble
* **SEK** - Swedish Krone
* **USD** - United States Dollar

.. warning::
    StarPass is only available as a payment method if you select "EUR" as the main currency.

6. Setting up Google reCAPTCHA (OPTIONAL)
--------------------------------------------
Google reCAPTCHA is a captcha system which prevents brute-force log in attempts. If you wish to only allow people to log in through Steam you can skip this step as it will have no benefit. If you wish to allow people to log in using a username and password, you should complete this to make your site more secure. To set it up go to https://www.google.com/recaptcha/admin and sign in using a Google account, or register if you don't have one. Where it says "Register a new site", enter anything you want under "Label" and enter your domain name under "Domains" and click register. On the next page, under "Keys" you will be given a Site Key and a Secret Key. Enter the Site Key next to ``$recaptchasitekey`` in "config.php" and the Secret Key next to ``$recaptchasecretkey``.

7. Creating the folder on your web host
------------------------------------------------
On your web host, in the public folder (usually called "public", "public_html" or sometimes just "www"), create a folder for SDonate to go in. Now, using FTP or your web host's build-in file browser upload everything from INSIDE the "web" folder into the folder you just created. When this is done, navigate to http://<yourdomain.tld>/<yourfolder>/install.php to complete installation, so if your domain is "myamazingdomain.com" and the folder you created is called "donate", you'd go to http://myamazingdomain.com/donate/install.php. If all is well it will just say "Installation complete!", and if not, it will tell you what is wrong.

You have now installed SDonate on your web server! You should look at the section on setting up payment information to accept payments.
