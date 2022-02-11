# Experimenting Github as a CMS 🧑‍🔬

This repo is the CMS for lembot static pages (except home page that I wanted highly customized):
- [/terms](https://lembot.com/terms)
- [/privacy](https://lembot.com/privacy)
- [/what-new](https://lembot.com/whats-new)
- [/blog](https://lembot.com/blog) & blog posts

## Why

Because

I ❤️ markdown : super simple to write and the result (header, link, paragraphe) is 100% predictible.

I ❤️ git : versioning comes for free.

I ❤️ writing markdown on github : `Add new file` -> `demo.md` -> start writing markdown / 👁️ preview / 💾 images hosting as simple as a drag-n-drop

## How

I am using [nextjs](https://nextjs.org/).

Building a website with nextjs is super easy and Vercel (the company behind nextjs) provide a blog sample code (see [here](https://github.com/vercel/next.js/tree/canary/examples/blog-starter-typescript)).

It is super easy, yes. But it's a bit of boilerplate code.

I wrapped this boilerplate code in simple functions like `getStaticPropsFromMarkdownFileUrl`, components like `<MarkdownPage />` and so.

Gonna share this soon.
