# Contact Form Helper #

## Overview ##

This module will create templates and fields which are related to functioning contact form feature. Idea of this module is simply saving time without creating fields and templates when it comes to usage.

### How to install ###

1. Copy the files for this module to /site/modules/ContactFormHelper/
2. In admin: Modules > Check for new modules. 
3. Click *install* for the Contact Form Helper. 

#### How to use ####
	
To get contact us form in your template use following block of scrip:
````````
<?php if($modules->isInstalled("ContactFormHelper")): ?>
	<?php echo $modules->get('ContactFormHelper')->getContactUsForm() ?>
<?php endif; ?>
`````````

Module use `add_contact_form_to_page` field as a switch to enable contact form feature. eg: Let say you need to include contact form in several pages.In this scenario you can add `add_contact_form_to_page` field to the required template. Use following code snippet:
`````````
<?php if($modules->isInstalled("ContactFormHelper")): ?>
<?php echo $modules->get('ContactFormHelper')->getConditionalContactUsForm() ?>
<?php endif; ?>
`````````







