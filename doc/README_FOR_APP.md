Launch-Soon
===========

Launch Soon is a Heroku-ready rails site that provides a viral launching soon page to collect users before your actual launch date.

You can deploy to Heroku, and immediately begin collecting email addresses in your Mailchimp list. The site provides a unique URL to each user who signs up, which keeps track of how many people they refer. The referral count and code are also stored in your Mailchimp list.


Pre-requisites
--------------

* A Mailchimp account with a list named "Interested"
* A Google Analytics Web Property ID (UA-#######-##)
* A Twitter account


Configuration
-------------

All configuration is done in the `app/controllers/application_controller.rb` file.  You are not required to touch any other files.

Mailchimp Setup:

1. Go to https://admin.mailchimp.com/lists/
2. Click the 'Create List' button
3. Name the list 'Interested' (the rest of the information is up to you)
4. Back at https://admin.mailchimp.com/lists/, click the Settings button for on the far right for the 'Interested' list
5. Select "List Fields and Merge Tags"
6. Change Field Labels to read:
 * Change "First Name" to "Referral Code", and change "FNAME" to "RCODE"
 * Change "Last Name" to "Referral Count", and change "LNAME" to "RCOUNT"