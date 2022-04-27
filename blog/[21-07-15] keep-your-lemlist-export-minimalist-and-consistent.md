---
head:
  title: "Keep your lemlist export minimalist and consistent - Lembot Blog"
  description: "Discover how to export only the data you care about. Lembot allows you to re-shape the lemlist export so your sheet stays minimalist and consistent."
card:
  title: "Keep your lemlist export minimalist and consistent"
  description: "Discover how to export only the data you care about. Lembot allows you to re-shape the lemlist export so your sheet stays minimalist and consistent."
coverUrl: "https://images.unsplash.com/photo-1550432163-9cb326104944"
emoji: "🎓"
date: "2021-07-15"
author:
  name: "François Rouault"
  imageUrl: "https://lh3.googleusercontent.com/ogw/ADea4I7LJjF5U_yHFaLQIoNCysLkiEHPLHnWKxj0i1SadVY=s32-c-mo"
  href: "https://www.linkedin.com/in/francoisrouault/"
tag: "how to"
---

# Keep your lemlist export minimalist and consistent

With lembot, you can choose between extracting all the CSV or only a set of columns.

![lembot extract mode options](https://user-images.githubusercontent.com/2499356/165461298-1944ed5e-b4c5-43bf-b672-3a734df60afd.jpg)

## Extract all

When choosing "All columns", lembot will import in your GSheet the lemlist CSV report **as is**. No more no less.

The end result is the same as if you had done the export and import manually.

## Or, choose your outputs

Why should I select columns?

This has 2 major advantages:

- Minimalist: your sheet gets easier too read because free of unnecessary data
- Consistent: the structure of your sheet won't change. If one day, the lemlist export template changes (for example, lemlist adds columns to the CSV) then your formula could be affected.

When you select columns, the export stay consistent over time. So does your formula 😉

There is two ways to choose your output: select columns or write columns.

### Select columns

While creating or editing a bot, click "Select columns".
 
Lembot will automatically detect your campaign CSV header and displays them in a table.

Once detected you can select which columns to extract, then click Continue to confirm your selection and finalize your bot.

![select columns](https://user-images.githubusercontent.com/2499356/151677443-7fd360fd-0c5c-4129-9297-6dd5703d969a.jpg)

### Write columns

This is a bit more advanced, yet very powerful feature. It lets you shape exactly your final output in your GSheet.

While creating or editing a bot, click "Write columns".

Start typing and see the column preview update automatically.

![write columns](https://user-images.githubusercontent.com/2499356/165496834-70d8807c-202a-43e6-a1d4-0470e8a01d05.jpg)

### Edit your selection at any moment

Note that you can edit your extract mode (all columns, select columns, or write columns) and your columns selection at any moment.

## Run export 🎉

Click "Run export" to only export the selected variables to your Google Sheets.

![choose_outputs_done](https://user-images.githubusercontent.com/2499356/151677451-2ab9b26e-21a9-4f70-aa15-ee573caa2300.jpg)

As you can see on the right, the sheet has only 4 columns as requested: `email`, `sentStep`, `sentAt` and `interestedAt`.

## Demo

![demo select outputs](https://user-images.githubusercontent.com/2499356/151677420-57011d17-11bd-4047-95b2-0879a3afb883.mp4)

---

Cheers,

François
