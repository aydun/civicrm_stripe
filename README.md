CiviCRM Stripe Payment Processor
--------------------------------
Version 1.8+ of this extension *must* use Stripe's latest API version (at least 2013-12-03).  
This is the API setting within your stripe.com account settings (just a button to upgrade).  
More info on how to change:  https://stripe.com/docs/upgrades#how-can-i-upgrade-my-api  

FIX ME
------
The current state of this payment processor may not be stable.  
It needs to be thoroughly checked for compatibility with the latest version(s) of CiviCRM 4.4.  

CONFIGURATION
-------------
All configuration is in the standard Payment Processors settings area in CiviCRM admin.  

GOOD TO KNOW
------------
Your CiviCRM 'Resource URLs' must be set to the extensions directory  
relative to Drupal/CRM base.  Example: /sites/all/civicrm_extensions/  
*NOT the full server path like /var/www/sites/all/civicrm_extensions/*  
This is the admin page for Resource URLs:  /civicrm/admin/setting/url  

There are multiple versions of this extension available.  This is:  
4.4:  Extension for CiviCRM 4.4.  
You do not need the CMS module for 4.4  

WEBHOOK
---------
The Webhook.php file is registered to the path of civicrm/stripe/webhook  
You will have to make a Webhook rule in your Stripe.com account and enter this path for recurring charges to end!  
For Drupal:  https://example.com/civicrm/stripe/webhook  
For Joomla:  https://example.com/index.php/component/civicrm/?task=civicrm/stripe/webhook  

INSTALLATION
------------
For CiviCRM 4.4:  
1)  Install extension.  
2)  Copy Stripe's PHP library folder 'stripe-php' to civicrm/packages/stripe-php  
You can get Stripe's PHP library here: https://github.com/stripe/stripe-php  

AUTHOR INFO
-----------
Joshua Walker  
http://drastikbydesign.com  
https://drupal.org/user/433663  
