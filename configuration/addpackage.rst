Adding a Package
===================

To add a package, open the SDonate admin dashboard, then go to the "Package Manager", then click the "Add Package" button. Select the game your server is for, then change the following settings:

* **Title** - Enter the title to give your package.

* **Description** - Enter a description for your package.

* **Image** - You can optionally upload an image for this package's icon. If you leave this blank the default game image will be used.

* **Pay What You Want** - If this is enabled the user will be able to choose how much they want to pay. The price they enter must be equal to or higher than the "Price" setting.

* **Price** - Enter the price of this package. If "Pay What You Want" is enabled, this will be the minimum price they must pay.

* **Max Purchases** - This is the maximum number of times a user can purchase a package. Set this to 0 to allow infinite purchases.

* **Commands** - This is where you choose the actions to be ran when a user purchases this package. When adding a command, you can choose what servers this command will be run on. Note that this command will run once for *every* server ticked. You may have to enter parameters for this package also. For each paramater, you can tick "User Chooses" to allow users to enter their own parameters. More info on commands can be found in :doc:`commands/commands`.

* **Duration** - Enter how long this package should last in days. Set to 0 to never expire.
