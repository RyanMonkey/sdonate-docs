Actions - Rust
==========================

Custom Command
-------------------------------------

Run a console command on the server.

Parameters:

* Execution Time - Choose whether the command will run as soon as the purchase is complete or when the user next joins the server, for most commands you should choose "On Join" to make sure the commands runs properly.
* Command - The console command to run.
* Expiration Command - The command to run when the package expires or when the package is revoked.

Give Item
-------------------------------------

Give the purchaser X amount of a certain item.

Parameters:

* Item Shortname - The shortname of the item to give the user. You can find a list of these at http://docs.oxidemod.org/rust/#item-list.
* Amount - The amount to give.

Give Blueprint
-------------------------------------

Give the user a blueprint for a certain item.

Parameters:

* Item Shortname - The shortname of the item for the blueprint. You can find a list of these at http://docs.oxidemod.org/rust/#item-list.
