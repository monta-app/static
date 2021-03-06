# GDPR

Last updated: March 25, 2021

__This document is to descripe the how we handle data on behalf of users.__

And what options we have for users to control it.

All users can at any time reach out on gdpr@monta.app and ask questions about their data. Eg:

 - What data do we have stored around them
 - Ask to get some user data changed
 - Get all their data deleted

Inside Monta App, under Me -> Profile. "Request for data" and "Request to get deleted" is added as 2 buttons. 

 Data request are sent instantly, and delete requests are carefully handled within 10 business days
 
 ### What data is stored
 
 - First & last name (optional) - Used for user profile
 - Profile image (optional) - Used for user profile, building trust for other users
 - Email (optional) - Used for User profile
 - Phone (optional) - Used for 2-factor login
 - Language (optional, taken from device configuration) - Used for for communicating in best possible language
 - Country - Used for applying to local laws
 - IP address - Used for fraud detection & IP to coordinate when GPS is disabled / not ready
 - Device info (platform, os version, device) - Used for improving the app expirence. Eg if 1 problem only appears on iphone, but another on android only on samsung devices
 - Device location (optional, stored when using credit cards) - Used for fraud detection

_Besides the user data above, we store data inputted in forms and saved. Like charge points, favorites, reports, chat etc._

### Where is the data stored

Most data is stored in [Amazon web services, AWS](https://aws.amazon.com/). In following data centers

 - eu-west-01, Ireland

We are using a handful of data storages

 - Aurora, MySQL - Master database
 - Elastic search - Search engine for map + log files
 - Dynamo DB - Configs
 - Elastic cache, Redis - Caching, normally less than 12hours
 - S3 - Files like images

Besides Amazon web services, AWS. We are using following

 - [Pubnub](https://pubnub.com) - User to user chat messages - 30 days retention on messages
 - [Intercom](https://intercom.com) - Customer support chat message

### Who else have access to what data
 - [Laravel Vapor](http://vapor.laravel.com/) as automated deployment (CD) have access to all above
 - [Laravel Forge](http://forge.laravel.com/) as automated deployment (CD) have access to all above
 - [Elastic Cloud](https://cloud.elastic.co) is managing Elastic search
 - [Twilio](https://www.twilio.com) is provider of sms messages
 - [Firebase - Google](https://firebase.google.com/) is provider of Push notificions. For Iphone users Apple are having access also
 - [Firebase - Google](https://firebase.google.com/) is provider of crash reports for Iphone and Android
 - [Bugsnag](https://bugsnag.com/) is provider of crash reports for Backend
 - [Firebase - Google](https://firebase.google.com/) is provider of analytics for Iphone and Android
 - [Google Analytics](https://analytics.google.com/) is provider of analytics for website
 - Services providers selling subscriptions, will get access to required user data such as (Name, address, phone and email) when a subscription is pending or active

### Data retention, backup

We are backing up several times each day. And keeping the backups for 20 days.
