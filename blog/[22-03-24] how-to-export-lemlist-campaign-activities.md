---
head:
  title: "How to export lemlist activities - Lembot Blog"
  description: "Discover how to export your lemlist campaign activities: event types (sent, opened, clicked...), the date of the interaction, the lead, sender, clicked URL..."
card:
  title: "Export your lemlist campaign activities"
  description: "Discover how to export your lemlist campaign activities: event types like sent, opened, clicked, interested, with the exact date and time of the interaction, the lead, sender, clicked URL, everything."
coverUrl: "https://images.unsplash.com/photo-1550432163-9cb326104944"
emoji: "🎓"
date: "2022-03-24"
author:
  name: "François Rouault"
  imageUrl: "https://lh3.googleusercontent.com/ogw/ADea4I7LJjF5U_yHFaLQIoNCysLkiEHPLHnWKxj0i1SadVY=s32-c-mo"
  href: "https://www.linkedin.com/in/francoisrouault/"
tag: "how to"
---

# Lemlist Campaign Activities

If you want to deep dive into your data, you would probably want to analyze your campaign **activities**.

This is the most enriched data in lemlist.

Every single email sent, opened, clicked, URL clicked, etc. is an activity. And they are all timestamped.

![screenshot](https://user-images.githubusercontent.com/2499356/163671320-39f11758-9dbd-4d03-922b-fe6c5afdc223.png)

## How to Export Activities

Lemlist does not provide a way to export them.

Lembot does 😎

### Create a Bot

When creating a bot, you will be asked what type of data you want to export : reports or **activitites**.

![export lemlist activities - new bot](https://user-images.githubusercontent.com/2499356/163671763-176d55d2-23ee-4049-a62f-f9c153ee7485.jpg)

Follow the steps to finish creating bot:

- choose your lemlist team and campaign to export the activities from
- choose your Google spreadsheet, sheet and cell from which to import the activities
- eventually, schedule automatic export
- save the bot

![bot](https://user-images.githubusercontent.com/2499356/163679230-8a7e9dd5-47dc-4eea-93f0-e0344755c8cf.png)

### Click Run Bot

Few seconds later, all your campaign activities are exported in your gsheet.

See 👇

![activities exported in gsheet](https://user-images.githubusercontent.com/2499356/163671842-722bc6b8-1ef5-4807-898b-b7c5df9ac576.jpg)

## First Time Event

If you only care about the first occurence of an event, check out the column `isFirst`.

## Steps

The column `sequenceStep` tells you the step when the event occured.

Watch out, index starts at 0. Meaning that

- `0` means "step 1"
- `1` means "step 2"
- and so on.

## Clicked URL

If your prospect clicks on link in your email, an activity of type `emailsClicked` is created and the clicked URL is available in the column `extra.location`.

## Event Types

Here is the list of all the lemlist event types available in the export

- emailsSent
- emailsOpened
- emailsClicked
- emailsReplied
- emailsDone
- emailsBounced
- emailsFailed
- emailsUnsubscribed
- emailsInterested
- emailsNotInterested
- snoozed
- annotated
- aircallDone
- aircallCreated
- aircallEnded
- aircallInterested
- aircallNotInterested
- apiDone
- apiInterested
- apiNotInterested
- apiFailed
- linkedinVisitDone
- linkedinVisitFailed
- linkedinInviteDone
- linkedinSent
- linkedinOpened
- linkedinInviteAccepted
- linkedinInviteFailed
- linkedinSendFailed
- linkedinReplied
- linkedinInterested
- linkedinNotInterested
- linkedinDone
- manualDone
- manualInterested
- manualNotInterested
- paused
- resumed
- skipped
- contacted
- hooked
- attracted
- warmed
- interested
- skipped
- notInterested

---

Feel free if you have any questions,

Cheers,

François
