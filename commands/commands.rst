About Commands/Actions
============================

Command Variables
--------------------------
You can use the following variables in command parameters to replace it with the user's own info. Valid variables are as follows:

* **{{VAR=STEAMID}}** - The user's 64-bit Steam ID i.e. 76561197960287930

* **{{VAR=STEAMID32}}** - The user's 32-bit Steam ID i.e. STEAM_0:0:111010

* **{{VAR=STEAMID3}}** - The user's SteamID3 i.e. U:1:222020

* **{{VAR=STEAMUSERNAME}}** - The user's Steam username (NOTE: This should not be used to assign packages, since more than one user can have the same Steam username, this should only be used for things like sending a personalised message such as "Thanks for purchasing, {{VAR=STEAMUSERNAME}}")

* **{{VAR=Minecraft_Username}}** - The user's Minecraft username.

Creating User Choices
---------------------------
If you have ticked "User Chooses", you can create choices for the parameter. If you do not create any choices, the buyer will be able to enter anything they want, but if you create at least 1 choice they will have to choose between the options you define. When creating a choice, you have to enter a name, value and price. The name is what is displayed to the buyer when choosing, the value is the actual parameter value and the price is the amount added to the package price if this choice is chosen. For example, if creating a choice for the "DarkRP Add Money" command, if you enter the name as "Ten Thousand Dollars", value "10000" and price "0", this will add nothing to the base package price and will add $10000 to their DarkRP money if this option is chosen.

For more info on the actions available for various games see:
    * :doc:`gmod`
    * :doc:`minecraft`
    * :doc:`rust`
    * :doc:`other`
    * :doc:`special`
