---
head:
  title: "How to export your campaign stats - Lembot Blog"
  description: "Lembot helps you export your campaign stats and keep it up-to-date without a click."
card:
  title: "Export your campaign stats"
  description: "You can use this Google Sheets formula COUNTA(Z3:Z)/COUNTA($A3:$A) to compute your campaign stats, then Lembot will keep this data up-to-date by automatically the export."
coverUrl: "https://user-images.githubusercontent.com/2499356/209329800-3f3935ac-c184-4ecc-8399-8e2019775d7b.jpg"
emoji: "🎓"
date: "2023-07-10"
author:
  name: "François Rouault"
  imageUrl: "https://lh3.googleusercontent.com/ogw/ADea4I7LJjF5U_yHFaLQIoNCysLkiEHPLHnWKxj0i1SadVY=s32-c-mo"
  href: "https://www.linkedin.com/in/francoisrouault/"
tag: "how-to"
---

# Exporting Your Lemlist Campaign Stats

_Disclaimer: Currently, Lembot does not offer a dedicated way to export this specific data. However..._

Here's a step-by-step guide on how you can accomplish it once and for all. Start by creating a new bot and inserting the data, beginning from line **2**.

Once you have exported your data, navigate to the columns labeled `sentAt`, `repliedAt`, etc. (these columns indicate the dates when the emails were sent, replied to, etc.).

Focus on the cell above the `sentAt` cell (e.g., "AC1") and enter the following formula: `=COUNTA(AC3:AC)/COUNTA($A3:$A)`. That's it! 🎉

Next, you can copy this formula and extend it to the subsequent rows, just as demonstrated in the video below. By scheduling regular exports, you can ensure that your data remains up-to-date.

![campaign stats](https://github-production-user-asset-6210df.s3.amazonaws.com/2499356/252350415-f7aaf097-1956-4cf5-a7cf-1e51228fa1d4.mp4)

---

Cheers,

François.
