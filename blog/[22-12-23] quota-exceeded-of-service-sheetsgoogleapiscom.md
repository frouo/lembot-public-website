---
head:
  title: 'How to fix the "[429] Quota exceeded" error - Lembot Blog'
  description: "The Google API limits the number of read and write operations per minute per user in order to protect the service"
card:
  title: "Google API error - Quota exceeded for quota metric 'Read/Write requests' and limit 'Read/Write requests per minute per user' of service 'sheets.googleapis.com'"
  description: "The Google API limits the number of read and write operations per minute per user. Simply review the schedule of your bots and megabots and space them out at bit."
coverUrl: "https://user-images.githubusercontent.com/2499356/209329800-3f3935ac-c184-4ecc-8399-8e2019775d7b.jpg"
emoji: "💥"
date: "2022-12-23"
author:
  name: "François Rouault"
  imageUrl: "https://lh3.googleusercontent.com/ogw/ADea4I7LJjF5U_yHFaLQIoNCysLkiEHPLHnWKxj0i1SadVY=s32-c-mo"
  href: "https://www.linkedin.com/in/francoisrouault/"
tag: "help center"
---

# Google API error - [429] Quota exceeded of service 'sheets.googleapis.com'

## Why this error?

The Google API limits the number of read and write operations per minute per user.

You are very likely to reach that limit with automation, especially when automations trigger all at once at the very same time. Which happens if you have never changed the default schedule time (7:30am) when you create a bot or a megabot.

> Google API is used by millions of sites. We put limits and quotas on API requests to protect the system from receiving more data than it can handle, and to ensure an equitable distribution of the system resources. The limits and quotas are subject to change.

_source: [Limits and Quotas on API Requests - google.com](https://developers.google.com/analytics/devguides/config/mgmt/v3/limits-quotas)_

## How to fix it?

To fix this, I suggest you update your bots / megabots scheduling a little.

Go though your bots and megabots and space out their schedules a bit. Something like:

- 7:00am
- 7:05am
- ...
- 7:30am

---

Cheers,

François.
