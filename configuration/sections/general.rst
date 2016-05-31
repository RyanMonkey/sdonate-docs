General Settings
========================

"General Settings" contains settings which change how the store operate. An explanation of all the settings is below:

* **Maintenance Mode** - When you enable maintenance mode, users are unable to access the site to make purchases but the admin dashboard is still accessible.

.. note::
    If you've enabled maintenance mode and can't find your way back to the admin dashboard, just go to http://yourdomain.com/folder/dashboard.php. If you are using the one-click hosting and setup this will be at https://sdonate.com/stores/<yourdomain>/dashboard.php.

* **Login Mode** - This changes whether users are allowed to use username and password or Steam login, or whether they must log in using Steam only.

* **Payment Mode** - If set to default, users can purchase packages directly and pay as they are purchasing the package. If set to "Credit Only", users must purchase credit before using it to buy a package. The purpose of this is explained in :doc:`../paypal`.

* **PayPal Enabled** - Enables/disables PayPal payments.

* **PayPal Email** - The purpose of this is explained in :doc:`../paypal`.

* **PayPal Sandbox** - Enables/disables PayPal sandbox mode. When sandbox mode is enabled no money will actually be used so it's useful for testing, make sure it's disabled before going live though.

* **Credits Enabled** - If this is enabled users can purchase credits to purchase packages with. If "Payment Mode" is set to "Credit Only" this cannot be disabled.

* **Store Name** - Sets the name of the store that will appear on the store and on PayPal.

* **Store Logo** - Upload an image to use as the store's icon at the top right or select "Text" to simply use the store name as the logo.

* **Home Page Text** - Set the text that shows up on the homepage of your site.

.. note::
    The following settings will only appear if your main currency is set to EUR/Euros.

* **StarPass Enabled** - Enables/disables StarPass payments.

* **StarPass Access Page URL/StarPass Monetization Component URL/StarPass Protection Code** - The purpose of these is explained in :doc:`../starpass`.
