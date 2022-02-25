# Experimenting Github as a CMS 🧑‍🔬

This repo is the CMS for lembot static pages:

- [/terms](https://lembot.com/terms)
- [/privacy](https://lembot.com/privacy)
- [/whats-new](https://lembot.com/whats-new)
- [/blog](https://lembot.com/blog) & blog posts

## Motivation

Like me, you probably focus all your effort in building a 100% custom `index.ts` home page to make it as **salesy** as possible.

What for all other pages, thoses pages where only the content matters?

For those pages, I wanted an easy way to generate them, edit them, write new ones, etc.

Using **markdown** and **github** sounds the best option for me because:

* I ❤️ markdown: super simple to write and the result (headers, paragraphs, links) is 100% predictible
* I ❤️ git: versioning comes for free
* I ❤️ writing markdown on Github: the editor is smart enough 🧠, has a preview mode 👁️ and provides drag-n-drop free images hosting 🌆

## How

I am using [nextjs](https://nextjs.org/).

Building a website with nextjs is super easy and there are a lot of nextjs blog sample code out there (official [here](https://github.com/vercel/next.js/tree/canary/examples/blog-starter-typescript) for example).

Ok, it is super easy. But it's a bit of boilerplate code.

I wrapped this boilerplate code in simple functions like `getStaticPropsFromMarkdownFileUrl`, components like `<MarkdownPage />` and so.

Gonna share this soon.

Gonna be as simple as create a creating a `[...nextmd].tsx` file, init `NextMd` with your git repo, call `getStaticPaths` and `getStaticProps`, draw your layout, and that's it 🔥

![wip](https://user-images.githubusercontent.com/2499356/155738752-c17686a3-d572-4e72-8563-e70438bdde38.jpeg)

[Follow me on Twitter](https://twitter.com/frouo) if you are interested. I am building this in public.
