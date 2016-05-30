Installation - Minecraft Server
========================================

Before using SDonate with a Minecraft server you must install the SDonate Minecraft plugin on your server.

1. Extracting the plugin
-----------------------------
If you haven't already, download SDonate from ScriptFodder then open the "sdonate-minecraft-plugin" folder and extract "SDonate Plugin.jar" somewhere on your PC, preferably on your desktop for easy access.

2. Upload to your server and configure
-----------------------------------------------
Upload "SDonate Plugin.jar" into your Minecraft server's plugin directory then restart your server. You will probably get a lot of errors, don't worry, this is normal. In your Minecraft plugin directory there should be a folder called "SDonate_Plugin". Open this folder, and inside there is a file called "config.yml". Edit this file, making the following changes:

* Next to ``URL`` write the URL to your pluginapi.php file. If you installed SDonate using the free included one-click hosting and setup, go to https://sdonate.com and go to your account page, you will see the URL next to "Plugin API URL". If you installed SDonate's website on your own web server, the url is http://<yourdomain.tld>/<yourfolder>/pluginapi.php, so if my domain was "myamazingdomain.com" and the folder SDonate was installed in is called "donate", the URL would be http://myamazingdomain.com/donate/pluginapi.php.
* Next to ``Plugin API Key`` write your SDonate API you generated earlier. You can get it from your account page at https://sdonate.com.
* Next to ``IP`` write the IP of your Minecraft server. This must be in numeric form i.e. "123.53.24.63" and **NOT** a domain like "play.myamazingserver.com".
* Next to ``Port`` write the port your Minecraft server is running on. By default this is 25565.

.. note::
    If your server IP is something like 142.34.63.124:25565 the IP is the part **before** the ``:`` and the port is the part **after** the ``:``. So in this case ``IP`` would be "142.34.63.124" and ``Port`` would be "25565".

3. Restart your server
----------------------------
Save all your changes to "config.yml", then restart your Minecraft server.


.. note::
    After you've finished installing the plugin to your Minecraft server you will still need to follow the instructions in :doc:`../configuration/addserver`.
