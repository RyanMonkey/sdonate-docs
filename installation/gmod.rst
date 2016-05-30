Installation - Garry's Mod Addon
========================================

Before using SDonate with a Garry's Mod server you must install the SDonate Garry's Mod addon on your server.

1. Extracting the addon
-----------------------------
If you haven't already, download SDonate from ScriptFodder then extract the "sdonate-gmod-plugin" folder somewhere on your PC, preferably on your desktop for easy access.

2. Configuring the addon
----------------------------
Go into the extracted "sdonate-gmod-plugin" folder, then open the "lua" folder. Open the file called "sdonate_config.lua" using your text editor. In the quotation marks next to ``SDonateURL`` enter the URL of your pluginapi.php file. If you installed SDonate using the free included one-click hosting and setup, go to https://sdonate.com and go to your account page, you will see the URL next to "Plugin API URL". If you installed SDonate's website on your own web server, the url is http://<yourdomain.tld>/<yourfolder>/pluginapi.php, so if my domain was "myamazingdomain.com" and the folder SDonate was installed in is called "donate", the URL would be http://myamazingdomain.com/donate/pluginapi.php. Now, in the quotation marks next to ``SDonateAPIKey`` enter your SDonate API key you generated earlier, and next to ``SDonateServerIP`` enter your Garry's Mod server's IP and next to ``SDonateServerPort``. The default chat command to open your donation store website is "!donate", but if you want to change this to something else change ``SDonateCommand``.

.. note::
    If your server IP is something like 142.34.63.124:27015 the IP is the part **before** the ``:`` and the port is the part **after** the ``:``. So in this case ``SDonateServerIP`` would be "142.34.63.124" and ``SDonateServerPort`` would be "27015".

3. Upload to your server
----------------------------
Save all your changes to "sdonate_config.lua", then upload the "sdonate-gmod-plugin" folder to your Garry's Mod server's addon folder, then restart your Garry's Mod server.

.. note::
    After you've finished installing the addon to your Garry's Mod server you will still need to follow the instructions in :doc:`../configuration/addserver`.
