# Experimenting Github as a CMS 🧑‍🔬

This repo is the CMS for lembot static pages (except home page that I wanted highly customized):
- [/terms](https://lembot.com/terms)
- [/privacy](https://lembot.com/privacy)
- [/what-new](https://lembot.com/whats-new)
- [/blog](https://lembot.com/blog) & blog posts

## why?

I ❤️ markdown : it's super fast to write and you know precisely how it will be rendered.

I ❤️ git : versioning comes for free.

I ❤️ writing markdown on github : `Add new file` -> `demo.md` -> start writing markdown / 👁️ preview / 💾 images hosting as simple as a drag-n-drop

## how?

lembot.com is coded from scratch with [nextjs](https://nextjs.org/).

Blog with nextjs is easy (see example [here](https://github.com/vercel/next.js/tree/canary/examples/blog-starter-typescript)) but it's a bit of boilerplate code.

I wrapped this boilerplate code in simple functions like `getStaticPropsFromMarkdownFileUrl`, components like `<MarkdownPage />` and so.

Gonna share this soon.
