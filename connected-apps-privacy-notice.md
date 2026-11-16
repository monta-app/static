CONNECTED APPS PRIVACY NOTICE
=============================

Monta ApS  
Strandboulevarden 122, 2100 Copenhagen, Denmark  
Email: info@monta.com  
Company registration number: 41668385


## 1. About this notice

This notice supplements Monta's [Privacy Policy](https://monta.com/en/legal-risk-compliance/privacy-policy/). It covers the optional apps that a Monta customer can connect to their Monta account ("connected apps"). Each section below covers one connected app.

In this notice, "Monta", "we", "us" and "our" mean Monta ApS. "You" means the Monta customer, and the person who connects an app for the customer.

Connecting an app is optional. You can disconnect it at any time.

Where this notice says nothing, the Privacy Policy applies.

## 2. Google Calendar

The Google Calendar app puts your scheduled Field Service jobs in Google Calendar, each with a Google Meet link. You connect a Google account in Monta Hub, on the Google Calendar page of the Application Marketplace.

### 2.1 What Monta asks Google for

When you connect a Google account, Monta asks Google for these permissions:

- `https://www.googleapis.com/auth/calendar.app.created`: to create one secondary calendar, called "Monta jobs", in the account, and to create, change and delete events in that calendar.
- `openid` and `https://www.googleapis.com/auth/userinfo.email`: to identify the connected account by its email address.

Monta can't see the account's other calendars, or the events in them.

### 2.2 What Monta receives from Google and keeps

- The email address of the connected Google account.
- The permissions you granted.
- The OAuth tokens Google issues, which let Monta manage the Monta jobs calendar.
- The ID of the Monta jobs calendar.
- For each event Monta creates: its ID, its link in Google Calendar, and its Google Meet link and meeting code.

To keep its events up to date, Monta reads only the Monta jobs calendar and the events Monta created in it.

### 2.3 What Monta sends to Google

Monta sends your own job data to Google, on your instruction. For each scheduled job, Monta creates an event with:

- a title with the job number, the job type and the name of the Location;
- the job's scheduled start and end;
- the street address of the site;
- a description with the job's title, type and priority, its EVSEs, the instructions for the technician and a link to the job in Monta Hub. It also has the job's technician link, unless you turn this off in your settings;
- the email addresses of the guests your settings invite: the job's recipients (by default, the service partner's contacts), the user the job is assigned to, and any extra attendees you add;
- a request for a Google Meet link.

Monta never sends the job's internal notes, the site's access details (such as gate or door codes), the technician link's passcode or the job's costs.

### 2.4 How Monta uses this information

Monta uses this information only to:

- create, update and cancel job events, with their Google Meet links, in the Monta jobs calendar;
- show in Monta Hub which account is connected and its status, and for each job, whether its event is in the calendar and its Google Meet link;
- show the Google Meet link on the job's technician page.

### 2.5 How Monta stores and protects this information

Monta stores this information in its databases on Amazon Web Services (AWS), in the EU (Ireland).

Monta encrypts the OAuth tokens with AWS Key Management Service (KMS) envelope encryption. Only the Monta service that calls Google can decrypt them. Monta Hub never shows them.

### 2.6 Disconnecting, and what Monta keeps

You can disconnect a Google account in Monta Hub at any time. When you do, Monta:

- revokes its access at Google;
- deletes the OAuth tokens;
- stops writing to the Monta jobs calendar.

If Google can't revoke the access at that moment, the account stays connected and Monta Hub tells you, so you can try again.

When you disconnect the account your Field Service jobs use, you can choose to first remove the events of upcoming jobs from the calendar. Past events always stay. The Monta jobs calendar, and any events left in it, stay in your Google account. You can delete them in Google Calendar.

After you disconnect, Monta keeps a record that the account was connected: its email address and the ID of the Monta jobs calendar. Jobs whose events stay in the calendar keep the event's ID, its link and its Google Meet link, until the job is deleted.

You can also remove Monta's access in your Google account, at [https://myaccount.google.com/permissions](https://myaccount.google.com/permissions). Monta can then no longer use the account. The next time Monta tries, Monta Hub marks the account as needing to be reconnected. To also delete the tokens Monta holds, disconnect the account in Monta Hub.

### 2.7 Sharing and limited use

Monta does not sell this information. Monta does not share it with third parties, except the service providers Monta needs to run the app, such as AWS for hosting, or where the law requires it.

Monta does not use this information for advertising. Monta does not use it to develop, improve or train generalised artificial intelligence or machine learning models.

Monta's employees do not read this information, except where needed for security purposes, to comply with applicable law, or with your consent to help you with a support request.

Monta's use and transfer of information received from Google APIs will adhere to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

## 3. Questions

If you have any questions about this notice, or you wish to exercise your rights as described in the Privacy Policy, you can contact Monta at info@monta.com.

## 4. Amendments to this notice

Monta may update this notice, for example when we add a connected app. Below is the date of the most recent version.

Date of the most recent version of this notice: 16 November 2026.
