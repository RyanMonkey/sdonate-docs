Special Actions
==========================

Important Notes
-------------------------------------

RCON commands are ran as soon as the buyer purchases the package, for this reason it is recommended that you DO NOT use commands that require the user to be connected to the server, as they will not work if the user is not connected to the game server when they are making a purchase. Test commands using the "Test Server" button to see which commands work. Use "Custom Command" instead of "RCON Console Command" if the Sourcemod plugin is installed.

MySQL Query
-------------------------------------

.. warning::
    Only use this if you absolutely know what you are doing, incorrect usage of this command can have very bad side effects. If you need help with this create a support ticket on [ScriptFodder](https://scriptfodder.com/scripts/view/2168).

Perform a query on a MySQL database.

Parameters:

* DB Host - The hostname the MySQL server is running on
* DB Name - The name of the database
* DB Username/DB Password - The username and password of the user used to access the database
* DB Query - The query - you can use prepared values by replacing values to prepare with a `?`
* DB Prepared Values - The values to be prepared, seperated by a `|NEWVAL|`

Custom Command (REQUIRES SOURCEMOD PLUGIN)
-------------------------------------

Run a console command on the server.

Parameters:

* Execution Time - Choose whether the command will run as soon as the purchase is complete or when the user next joins the server, for most commands you should choose "On Join" to make sure the commands runs properly.
* Command - The console command to run.
* Expiration Command - The command to run when the package expires or when the package is revoked.
