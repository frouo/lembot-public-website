---
head:
  title: 'How to fix the "limit of 10000000 cells" error - Lembot FAQ'
  description: "The Google Sheets API limits the number of cells per spreadsheet. The limit is set at 10 million cells per spreadsheet."
card:
  title: "Google API error - This action would increase the number of cells in the workbook above the limit of 10000000 cells"
  description: "This is a Google API limitation for spreadsheets, they are limited to 10 million cells. Consider using 2 spreadsheets instead of 1, or reducing the number of campaigns in your megabots"
coverUrl: "https://user-images.githubusercontent.com/2499356/209329800-3f3935ac-c184-4ecc-8399-8e2019775d7b.jpg"
emoji: "💥"
date: "2022-12-23"
author:
  name: "François Rouault"
  imageUrl: "https://lh3.googleusercontent.com/ogw/ADea4I7LJjF5U_yHFaLQIoNCysLkiEHPLHnWKxj0i1SadVY=s32-c-mo"
  href: "https://www.linkedin.com/in/francoisrouault/"
tag: "error"
---

# Google API error - [400] Invalid requests[0].pasteData: This action would increase the number of cells in the workbook above the limit of 10000000 cells.

![Google Sheets limit of 10000000 cells](https://user-images.githubusercontent.com/2499356/209356372-4f453aba-b3d0-4b6b-a3d8-2036481ad23e.jpg)

## Why this error?

Import to Google Sheets failed because this action would exceed the max limit of 10 million cells per spreadsheet.

This is a Google API limitations for spreadsheets:

> Up to 10 million cells or 18,278 columns (column ZZZ) for spreadsheets that are created in or converted to Google Sheets.

_source: [Files you can store in Google Drive - google.com](<https://support.google.com/drive/answer/37603#:~:text=Up%20to%2010%C2%A0million%20cells%20or%2018%2C278%C2%A0columns%20(column%20ZZZ)%20for%20spreadsheets%20that%20are%20created%20in%20or%20converted%20to%20Google%20Sheets>)_

## How to fix it?

Here are some ways to avoid this error:

- Move sheet in another spreadsheet
- Reduce the number of campaigns in your megabot

## Pay attention, 10000000 cells per spreadsheet (not sheet)

A Google spreadsheet is made of multiple sheets.

The limitation applies to the spreadsheet, to the sum of the cells of its sheets.

![spreadsheet and its sheets](https://user-images.githubusercontent.com/2499356/209376677-4fabb247-8cd7-4bcd-b871-26b745420517.jpg)

---

Cheers,

François.
