# GDPR

Monta ApS

Strandboulevarden 122, 2100 Copenhagen, Denmark

info@monta.app

Company registration number: 41668385

**Last updated: 30 November 2021**

This document is to describe how we handle data on behalf of users. This compliments our [Privacy Policy](https://app.monta.app/privacy-policy).

You are entitled to the following:

- The right to access – You have the right to request copies of your personal data.

- The right to rectification – You have the right to request that Monta correct any information you believe is inaccurate. You also have the right to request Monta to complete the information you believe is incomplete.

- The right to erasure – You have the right to request that Monta erase your personal data, under certain conditions.

- The right to restrict processing – You have the right to request that Monta restrict the processing of your personal data, under certain conditions.

- The right to object to processing – You have the right to object to Monta&#39;s processing of your personal data, under certain conditions.

- The right to data portability – You have the right to request that Monta transfer the data that we have collected to another organization, or directly to you, under certain conditions.

Inside of the Monta App, it is possible to [request your data and request to delete your account](https://intercom.help/monta-aps/en/articles/4831492-i-would-like-to-delete-my-account).

The requests are handled as soon as possible and usually within 10 business days.

**What data is stored**

- First &amp; last name (optional) - Used for user profile

- Profile image (optional) - Used for user profile

- Email (optional) - Used for User profile

- Phone (optional) - Used for 2-factor login

- Language (optional, taken from device configuration) - Used for for communicating in your preferred language

- Country - Used for complying to local laws and regulations

- IP address - Used for fraud detection &amp; IP to coordinate when GPS is disabled / not ready

- Device info (platform, OS version, device model) - Used for improving the app experience and troubleshooting

- Device location (optional, stored when using credit cards) - Used for fraud detection

- We also store data that users input themselves in forms and other features, such as your favorite charge points or customer support contact.

**Where is the data stored**

Most of our data is stored in Amazon Web Services, AWS (EKS / EC2) in the following data center: eu-west-1 in Ireland.

We are using a handful of data storages:

- Aurora, MySQL - Master database

- Elastic search - Search engine for map + log files

- Dynamo DB - Configs

- Elastic cache, Redis - Cached data, mainly for PHP app. Normally less than 12 hours.

- S3 - Files like images

- Pubnub - User to user chat messages - 30 days retention on messages

- Intercom - Customer support chat messages

**Services used**

- Laravel Vapor as automated deployment (CD) have access to all above.

- Laravel Forge as automated deployment (CD) have access to all above.

- Elastic Cloud is managing Elastic search.

- Twilio is the provider of sms messages.

- Firebase by Google is the provider of push notifications. For iPhone users Apple also has access.

- Firebase by Google is the provider of crash reports for iPhone and Android.

- Bugsnag is the provider of crash reports for Backend.

- Firebase by Google is the provider of analytics for both iPhone and Android.

- Google Analytics is the provider of analytics for our websites.

- Service providers selling subscriptions will get access to only the minimum required user data needed such as name, address, phone and email when a subscription is pending or active.

- Stripe handles credit card and banking information.

- Elasic.co: Logging data

- Sentry: Crash data

- Snowflake (Ireland): Big data

- Weld (Ireland): Sync data to Snowflake

- Microsoft PowerBI

Internal tools (Hosted inside our K8s cluster):

- Grafana Loki keeps logging data.

- Elastic Search

**Backups**

We are backing up several times each day and keep our backups for 20 days.

**Contact us**

If you have any questions about the data we hold on you or you would like to exercise one of your data protection rights, please do not hesitate to contact us.
