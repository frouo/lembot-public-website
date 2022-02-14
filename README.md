# Experimenting Github as a CMS 🧑‍🔬

This repo is the CMS for lembot static pages:

- [/terms](https://lembot.com/terms)
- [/privacy](https://lembot.com/privacy)
- [/whats-new](https://lembot.com/whats-new)
- [/blog](https://lembot.com/blog) & blog posts

## Why

I wanted a full custom home page for my website (`index.ts`), and an easy way to generate all the "more common" pages.

Using markdown and github because:

I ❤️ markdown : super simple to write and the result (header, link, paragraphe) is 100% predictible.

I ❤️ git : versioning comes for free.

I ❤️ writing markdown on github : `Add new file` -> `demo.md` -> start writing markdown / 👁️ preview / 💾 drag-n-drop images hosting

## How

I am using [nextjs](https://nextjs.org/).

Building a website with nextjs is super easy and there are lots of nextjs blog sample code (official [here](https://github.com/vercel/next.js/tree/canary/examples/blog-starter-typescript) for example).

It is super easy, yes. But it's a bit of boilerplate code.

I wrapped this boilerplate code in simple functions like `getStaticPropsFromMarkdownFileUrl`, components like `<MarkdownPage />` and so.

Gonna share this soon.

Gonne be as simple as copy/pasting the `[nextmd].ts` file in your project.

```
pages/
  - [...nextmd].ts
```
