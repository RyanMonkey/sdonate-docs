Installation - Rust Oxide Plugin
========================================

Before using SDonate with a Rust server you must install the SDonate Oxide plugin on your server.

1. Extracting the plugin
-----------------------------
If you haven't already, download SDonate from ScriptFodder then open the "sdonate-rust-plugin" folder and extract "SDonate.cs" somewhere on your PC, preferably on your desktop for easy access.

2. Upload to your server and configure
-----------------------------------------------
Upload "SDonate.cs" into the "oxide/plugins" directory then restart your server. Now, in the "oxide" folder there should also be a folder called "config", and inside the "config" folder is a file called "SDonate.json". Open this file and make the following changes:

* Next to ``PluginAPIUrl`` write the URL to your pluginapi.php file. If you installed SDonate using the free included one-click hosting and setup, go to https://sdonate.com and go to your account page, you will see the URL next to "Plugin API URL". If you installed SDonate's website on your own web server, the url is http://<yourdomain.tld>/<yourfolder>/pluginapi.php, so if my domain was "myamazingdomain.com" and the folder SDonate was installed in is called "donate", the URL would be http://myamazingdomain.com/donate/pluginapi.php.
* Next to ``SDonateAPIKey`` write your SDonate API you generated earlier. You can get it from your account page at https://sdonate.com.
* Next to ``ServerIP`` write the IP of your Rust server. This must be in numeric form i.e. "123.53.24.63" and **NOT** a domain like "play.myamazingserver.com".
* Next to ``ServerPort`` write the port your Rust server is running on. By default this is 28015.

.. note::
    If your server IP is something like 142.34.63.124:28015 the IP is the part **before** the ``:`` and the port is the part **after** the ``:``. So in this case ``IP`` would be "142.34.63.124" and ``Port`` would be "28015".

3. Restart your server
----------------------------
Save all your changes to "SDonate.json", then restart your Rust server.


.. note::
    After you've finished installing the plugin to your Rust server you will still need to follow the instructions in :doc:`../configuration/addserver`.
