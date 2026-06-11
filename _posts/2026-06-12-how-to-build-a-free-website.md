---
layout: post
title: "How to Build a Website and Launch Your First Blog for Completely Free using Github Pages"
date: 2026-06-12
---

Starting your own corner of the internet usually comes with a catch: expensive monthly hosting fees, domain renewals, or restrictive platform rules. But what if you could build a professional, highly customizable blog completely for free, with zero hosting costs forever? 

That is exactly what we are doing today using **GitHub Pages** and **Jekyll**. 

This guide covers the exact blueprint to take you from a blank repository to a live, discoverable website—all handled directly inside your web browser.

---

## The Stack: GitHub Pages + Jekyll

Before diving in, let's look at the tools we are using:
* **GitHub Pages:** A free hosting service provided by GitHub that turns code repositories into live public websites.
* **Jekyll:** A static site generator. Instead of writing raw HTML code for every single blog post, Jekyll lets you write simple Markdown text files and automatically converts them into a beautiful, structured website.

---

## Step 1: Claim Your Corner of the Web

Every GitHub account gets one special repository dedicated to web hosting. 

1. Create a new GitHub repository.
2. Name it exactly: `<your-username>.github.io` (For example, mine is `tqnhu2407.github.io`).
3. Set the repository visibility to **Public** and initialize it with an empty `README.md`.

Naming the repository exactly like this tells GitHub to instantly activate its web hosting servers for your account.

---

## Step 2: Configure the Jekyll Engine

Next, we need to give Jekyll a set of instructions so it knows how to style our blog. We do this with a configuration file.

1. In your repository, click **Add file** -> **Create new file**.
2. Name the file exactly: `_config.yml`
3. Paste the following configuration code inside:

```
title: My Personal Blog
description: A place where I share my thoughts, guides, and projects.
theme: minima
```

4. Click Commit changes to save the file.

**What is Minima?** Minima is Jekyll's official, beautifully minimalist default theme. It includes a clean layout, dark mode compatibility, and built-in mobile responsiveness out of the box.

---

## Step 3: Create the Homepage

We need a landing page that will act as the "front door" of our blog.

1. Create a new file named `index.md` (make sure to delete your old index.html if you have one, as it will block Jekyll).
2. Paste this exact code into it:

```
---
layout: home
---

Welcome to my website! Check out my latest blog posts below.
```

3. Commit changes. The `layout: home` instruction tells Jekyll to automatically generate a chronological feed of your blog posts right on the homepage.

## Step 4: Write Your First Post

Jekyll organizes all your articles inside a specific folder. It also enforces a strict naming convention for posts: `YYYY-MM-DD-title.md`.

1. Click Add file -> Create new file.
2. Type `_posts/` into the name box to create a folder, then finish the filename so it looks like this: `_posts/2026-06-12-hello-world.md`
3. Add the layout details (Front Matter) and your content:

```
---
layout: post
title: "Hello World: Welcome to My Free Blog!"
date: 2026-06-12
---

This is my very first blog post, published completely for free using GitHub Pages! 

Writing future posts will be as simple as adding new Markdown files to this `_posts` folder. Jekyll handles all the archiving, formatting, and linking automatically.
```

4. Commit changes.

## Your Site is Live!

Give GitHub about 60 seconds to compile your code, then open a new tab and head over to your custom URL. You now officially own a lightning-fast, secure, and completely free blogging platform!
