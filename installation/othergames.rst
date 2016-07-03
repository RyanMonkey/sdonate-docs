Installation - Sourcemod Plugin
========================================

.. note::
    Sourcemod is only used for CS:GO, TF2 and L4D2.
    Installing the Sourcemod plugin is optional, however without it you will be unable to use expiration commands.

1. Extracting the plugin
-----------------------------
If you haven't already, download SDonate from ScriptFodder then extract the "sdonate-sourcemod-plugin" folder somewhere on your PC, preferably on your desktop for easy access.

2. Upload to your server and configure
-----------------------------------------------
Upload everything INSIDE the "sdonate-sourcemod-plugin" folder into "/addons/sourcemod" on your server. Now, restart your server and go to "cfg/sourcemod", in here should be a file called "sdonate.cfg", open it and edit the settings as follows:

* Next to ``sdonate_apikey`` write your SDonate API you generated earlier. You can get it from your account page at https://sdonate.com.
* Next to ``sdonate_serverip`` write the IP of your server. This must be in numeric form i.e. "123.53.24.63" and **NOT** a domain like "play.myamazingserver.com".
* Next to ``sdonate_serverport`` write the port your server is running on. By default this is 27015.
* Next to ``sdonate_url`` write the URL to your pluginapi.php file. If you installed SDonate using the free included one-click hosting and setup, go to https://sdonate.com and go to your account page, you will see the URL next to "Plugin API URL". If you installed SDonate's website on your own web server, the url is http://<yourdomain.tld>/<yourfolder>/pluginapi.php, so if my domain was "myamazingdomain.com" and the folder SDonate was installed in is called "donate", the URL would be http://myamazingdomain.com/donate/pluginapi.php.

.. note::
    If your server IP is something like 142.34.63.124:28015 the IP is the part **before** the ``:`` and the port is the part **after** the ``:``. So in this case ``IP`` would be "142.34.63.124" and ``Port`` would be "28015".

3. Reload The Plugin
----------------------------
Save all your changes to "sdonate.cfg", then either use the command "sm plugins reload sdonate" in your SERVER console, or just restart the server.


.. note::
    After you've finished installing the plugin to your Rust server you will still need to follow the instructions in :doc:`../configuration/addserver`.
