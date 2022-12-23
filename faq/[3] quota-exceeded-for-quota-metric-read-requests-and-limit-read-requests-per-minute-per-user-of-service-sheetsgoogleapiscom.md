---
head:
  title: 'How to fix the "Read requests quota exceeded" error - Lembot FAQ'
  description: "The Google API limits the number or read per minute per user in order to protect the system and ensure equitable distribution"
card:
  title: "Google API error - Quota exceeded for quota metric 'Read requests' and limit 'Read requests per minute per user' of service 'sheets.googleapis.com'"
  description: "The Google API limits the number of read per minute per user. Simply review the schedule of your bots and megabots and space them out at bit."
coverUrl: "https://user-images.githubusercontent.com/2499356/209329800-3f3935ac-c184-4ecc-8399-8e2019775d7b.jpg"
emoji: "💥"
date: "2022-12-23"
author:
  name: "François Rouault"
  imageUrl: "https://lh3.googleusercontent.com/ogw/ADea4I7LJjF5U_yHFaLQIoNCysLkiEHPLHnWKxj0i1SadVY=s32-c-mo"
  href: "https://www.linkedin.com/in/francoisrouault/"
tag: "error"
---

# Google API error - [429] Quota exceeded for quota metric 'Read requests' and limit 'Read requests per minute per user' of service 'sheets.googleapis.com'

## Why this error?

The Google API limits the number of read per minute per user.

You are very likely to reach the limit with automation that runs at the very same moment, in other words **scheduled at the same time**.

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
