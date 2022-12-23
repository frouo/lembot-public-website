---
head:
  title: 'How to fix the "Duplicate headers found" error - Lembot FAQ'
  description: "Lembot found a duplicate in your custom variables. Open your campaign in the lemlist dashboard, review your custom variables and delete the duplicate."
card:
  title: "Duplicate headers found"
  description: "Lembot found a duplicate in your campaign custom variables. Review your custom variables in your Lemlist dashboard, found the duplicate and remove it."
coverUrl: "https://user-images.githubusercontent.com/2499356/209329800-3f3935ac-c184-4ecc-8399-8e2019775d7b.jpg"
emoji: "💥"
date: "2022-12-23"
author:
  name: "François Rouault"
  imageUrl: "https://lh3.googleusercontent.com/ogw/ADea4I7LJjF5U_yHFaLQIoNCysLkiEHPLHnWKxj0i1SadVY=s32-c-mo"
  href: "https://www.linkedin.com/in/francoisrouault/"
tag: "error"
---

# Duplicate headers found

![screenshot duplicate headers found error](https://user-images.githubusercontent.com/2499356/209323620-cec70d39-324c-4cc3-a2ce-b55b9e7d6c21.jpg)

## Why this error?

Lembot found multiple columns with the same name in the final export.

This happens when your campaign has a duplicate **custom variables**, or when your **custom variables** includes lemlist report reserved columns such as `openedAt`, `bouncedAt`, etc...

💡 Lembot does not take responsibility for choosing one variable over another and prefers to fail.

## How to fix?

Review your campaign's custom variables in the lemlist app, found the duplicates and clean them.

Fortunately, lembot helps you with that by listing the duplicates directly in the error message, between the square brackets.

### Common scenario

Let's take the example where lembot told me it found a duplicate for the column `["notes"]`. If I manually download the report and open the CSV, I can see that I have two columns named `notes`. Now I have to open the lemlist app, open the campaign, check its custom variables and delete the `notes` I don't need.

![lemlist CSV report](https://user-images.githubusercontent.com/2499356/209316545-d0403326-e467-411f-a7e2-314c2690d485.jpg)

### Tricky scenario

You will encounter this error if you use the same variables that lemlist uses in their reports. I'm talking about `sentStep`, `sentAt`, `repliedAt`, `bouncedAt`... This happens when you use a lemlist CSV report in order to import your leads when creating a campaign.

In the example below, lembot found duplicates for `bouncedAt`, `callDoneAt` and so. Indeed, I can see they are in my custom variables.

![reserved name](https://user-images.githubusercontent.com/2499356/209301742-942810f8-9436-4e5e-b358-0b5b41f94f18.jpg)

![my custom variables in the lemlist app](https://user-images.githubusercontent.com/2499356/209301527-d18c4623-5864-4ebb-8547-c0c62b432a4c.jpg)

Cheers,

François.
