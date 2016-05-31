Actions - Garry's Mod
==========================

**Console Command**

Run a console command on the player.

Parameters:

* Command - The console command to run.
* Package Expiry Command - The command to run when the package expires or when the package is revoked.

**Custom LUA**

Run a custom LUA command.

Parameters:

* LUA - The LUA code to run.
* Package Expiry LUA - The LUA code to run when the package expires or when the package is revoked.

**Add To Group**

Add the user to the specified group. Make sure to choose the right one for the admin mod your server is using.

Parameters:

* Rank - The rank to give the user. Note that for Assmod this must be the rank number and for all other mods it must be the rank name.

**DarkRP Add Money**

Give the user the specified amount of money in DarkRP.

Parameters:

* Money - The amount of money to give the user.

**DarkRP Custom Job**

Create a custom job in DarkRP.

Parameters:

* Job Name - The name of the job.
* Models - The file paths of the models available for this job separated by commas. Example - /path/to/model/model1.mdl,/path/to/model/model2.mdl,/path/to/model/model3.mdl If you want to offer the user a choice of models enter the path to each one in a seperate choice.
* Description - The job description.
* Weapons - The weapons this job spawns with separated by commas. Example - weapon_ak472, weapon_keypadchecker, lockpick If you want to offer the user a choice of weapons enter each one in a seperate choice.
* Salary - This job's salary.
* Has License - Whether this job has a weapon license. Enter 0 for no and 1 for yes.

**Pointshop 1 Points**

Give the user the specified amount points in Pointshop 1.

Parameters:

* Points - The amount of points to give the user.

**Pointshop 2 Standard Points**

Give the user the specified amount of standard points in Pointshop 2.

Parameters:

* Points - The amount of standard points to give the user.

**Pointshop 2 Premium Points**

Give the user the specified amount of premium points in Pointshop 2.

Parameters:

* Points - The amount of points to give the user.

**Send Chat Message to Buyer**

Put a message in the chatbox of the buyer.

Parameters:

* Message - The message to display in the user's chatbox.
* Expiration Message - The message to display in the user's chatbox when the package expires or is revoked.

**Send Chat Message to All Players**

Put a message in the chatbox of all players on the server.

Parameters:

* Message - The message to display in all players chatboxes.
* Expiration Message - The message to display in all players chatboxes when the package expires or is revoked.
