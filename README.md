This modification was developed 100% in the OCMOD format, and displays the custom fields:

In the store administration, viewing the delivery list, invoice and request.

In front of the store, in the editing of addresses in the client account and in the order confirmation e-mail.

### Installation

 1. Access the link: https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=23447
 2. Locate the file compatible with your version of OpenCart and download it.
 3. In the store administration, access the menu ** Extensions → Installer ** (Extensions → Installer), click the button ** Upload **, select the file ** ocmod-editor.ocmod.zip ** and wait for the completion of the automatic installation.
 4. After installation, access the menu ** Extensions → Modifications ** (Extensions → Modifications) and click twice on the ** Update ** button (Refresh), so that the installed modification is added in the store, remembering that it is not the ** Update ** button on the browser, but the ** Update ** button in blue next to the orange and red button on the OpenCart screen.
 5. ** Only in OpenCart 3 **, go to the main page of the store administration control panel, under the ** Exit ** button, you will see a blue button with the design of a white gear inside it, click on this button and in the popup that will open, click on the two orange buttons inside the ** Action ** column to update the theme cache.

### Configuration

After installing the modification, access the menu ** Settings → Auxiliary data → Countries ** (System → Localization → Countries), locate the country "** Brazil **" (locate the country Brazil), click the button "** Edit ** "(Edit), in the country data in the field" ** Address formatting ** "(Address Format) add the code below replacing in the {custom_field_ID} tag the text ** ID ** with the custom field id that can be found in the menu ** Customers → Customize registration ** (Customers → Custom Fields):

`` php
{firstname} {lastname}
{company}
{address_1}, {custom_field_ID}
{address_2}
{postcode}
{city} / {zone}
{country}
``

Since you can add as many custom fields as you want, remembering that all must be in the format {custom_field_ID}, and lastly click on the button ** Save ** (Save).

** Displaying custom fields in the checkout address selection: **

In OpenCart version 2:

[Manual] (./ manuals / OPENCART_2.md)

In OpenCart version 3:

[Manual] (./ manuals / OPENCART_3.md)

### Uninstallation

In OpenCart version 2:

Access the ** Extensions → Modifications ** menu, locate and select the modification with the name '** Custom fields for OpenCart **', then click the ** Delete ** button, and ** Refresh ** button.

In OpenCart version 3:

Access the menu ** Extensions → Installer ** (Extensions → Installer), locate the file ** ocmod-editor.ocmod.zip ** and click the button ** Uninstall **, then go to the menu ** Extensions → Modifications * * (Extensions → Modifications), click the ** Update ** button (Refresh), and finally go to the main page of the store administration control panel, under the ** Exit ** button, you will see a color button blue with the design of a white gear inside it, click on this button and in the popup that will open click on the two orange buttons that are inside the column ** Action ** to update the theme cache.

### Update

Access the store administration and perform the Uninstall procedure, then perform the Installation procedure.

### Doubts

OCMOD (OpenCart Modification) is native to OpenCart, that is, it is not necessary to install any add-on in OpenCart to use modifications or extensions in the OCMOD format, for more information about OCMOD, follow the link for more information:

https://github.com/opencart/opencart/wiki/Modification-System
