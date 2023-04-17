---
title: "First Post"
date: 2023-04-13T09:12:56+01:00
draft: false
tags: ["webdev"]
---

### Site is up!

I've spent a good few days writing this static site as though I don't have 5 assignments coming up, but it's very important to treat webdev as a hobby rather than an _actual_ technical pursuit. A few notes:
> I do not have spell check, and I cannot spell! So as it stands the site will be _rife_ will spelling errors.  

> I may not have true use for this blog, so who's to say as to whether it will be updated or not.  

> This site doesn't have any kind of latex compilation, which could be very important considering.  

> I intend to send prospective employers to this site so it has to be somewhat flattering. We'll see how that goes!  

The site has three themes (so far!): astral, frilly and department. Astral is pretty and acts as the default right now (it's called default everywhere in the source code), Frilly is based on [Light Ediands website](https://www.ediand.xyz/). The themes was a bit of a struggle for me because I don't really know anything about websites, so I was very confused as to how I could switch between stylesheets dynamically. I was under the impression that local storage/cache/cookeis etc were only accessible to dynamic webpages. As it stands the theme of the site is saved in javascripts localStorage dictionary. This variable also allows the logo in the bottom right corner to change.

I intend to put two more themes in, specifically gruvbox light and dark mode. I wrote the website with hugo site generation ([source here](https://github.com/oisindavey/oisindavey.github.io)), so I can update it pretty easily. Hugo has a feature called "Partials" which is like a little function you can write that generates html & markdown. For example the sidepanel navigation is a partial called on every page (although it's really called in another base structure which every page _has_ to call by default.) I'll write some more to help create blog posts, like one that inserts images etc.
