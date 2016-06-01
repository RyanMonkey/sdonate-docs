Email Settings
========================

"Email Settings" contains settings related to sending confirmation emails to your buyers. Instructions to enable sending emails to buyers are as follows:

1. You will need an email address to send emails from. You can use one from a provider such as GMail or Outlook, or you can use your own SMTP/mail server. Enter this email address in "Sending Email Address" and the password for this email account  in "Sending Email Password".

2. Enter the SMTP server, port and encryption protocol in the relevant boxes. Below are some SMTP details for major email providers:

+-------------------------------------+--------------------------------------------------+------+---------+
|Email Provider                       |SMTP Server                                       |Port  |Protocol |
+=====================================+==================================================+======+=========+
|GMail                                |smtp.gmail.com                                    |465   |SSL      |
+-------------------------------------+--------------------------------------------------+------+---------+
|Outlook/Live/Hotmail                 |smtp-mail.outlook.com                             |587   |TLS      |
+-------------------------------------+--------------------------------------------------+------+---------+
|Yahoo                                |smtp.mail.yahoo.com                               |465   |SSL      |
+-------------------------------------+--------------------------------------------------+------+---------+

3. In "Purchase Complete Email Subject" "Purchase Complete Email Subject" enter the subject and body text respectively to appear in purchase confirmation emails. You can use variables to replace text with information about the purchase, the valid variables are:

    * {{VAR=Username}} - The purchaser's username
    * {{VAR=Package}} - The name of the package they purchased
    * {{VAR=Store Name}} - Your store's name

4. Hit "Submit" to save.
