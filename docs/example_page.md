---
title: Example Page
layout: default
nav_order: 10
nav_exclude: true
authors:
  - key: kaj
    role: Nerd
  - key: example
authors_title: Authors but Cooler
authors_id: cool-authors
---

# Example Page
{: .fs-9 .no_toc }
This page is meant to use as a reference when making your own pages.
{: .fs-6 .fw-300 }

You won't find every single solution to your problems here, but there will be a lot of stuff that's good to know.  
Be sure to look at the page in markdown too, not just on the web. See how the markdown creates what's visible on the actual page.  
Anyway, let's get to it.

# Table of Contents
{: .no_toc }

- TOC
{:toc}
<!-- Here's how to add a comment -->
<!--
It can span multiple lines! Anything between those two tags will be ignored, and is only for taking notes essentially.

That thing up there above these comments btw is how to add a table of contents (TOC)
It automatically generates a list of all the headers in the page and makes links to them.
You'll notice that the first header (#Example Page) has a little tag below it { .no_toc }, which excludes it from the toc.
-->


<!--PAGES-->

# Pages
At the top of each page you can specify a bunch of information about a page. This is all that matters when it comes to where the page is located in the ancestry, meaning which page it's a child-page of, etc. Every page needs a section like this.  
You should specify:  
* **title:** The name of the page, which can differ from the file name itself.
* **parent:** The title of the page this page should be a child of. If this isn't set the page will be listed as a main page next to pages like About Us and Getting Started. You'll usually want to set this.
* **grand_parent:** If your page's parent title is used in multiple places (for example, there are three pages named "Compositing" under Glossary, Workflow and Tutorials) you'll want to specify which of these your page should be parented to by setting the grand_parent to the title of the page the parent is parented to. For example, if you're adding a page under `Tutorials & Guides / Compositing`, set the grand_parent to `Tutorials & Guides`.
* **layout:** Just set it to `default`. The alternative is `minimal`, which omits the side-bar to the left.
* **nav_order:** Pages with a higher value are sorted after pages with a lower value when they are siblings. Try to set this to a multiple of 10, so that if another page needs to be added between yours and the one beside it, there's still plenty of room before we need to change the nav_order value.
* **authors:** Read about Authors [further down this page](#authors).

There are a lot of things beside that which you *could* specify, but those are the most important ones. For more details read the [Just The Docs] documentation.


<!--TEXT-->

# Text
Text is really simple to write but it's not like writing in a regular text document.

Just doing a regular line-break between this line
and the next one
won't do what you expect.

But if I add  
two spaces after each line  
then the lines do break.  

You can also use <br> the HTML tag for a line-break, `<br>`

You can also use three dashes like this `---` to make a horizontal line, to more clearly divide sections. Or use `<hr>`

---

Wow, what a line.


<!--IMAGES & VIDEOS-->

# Images & Videos

The simplest way to add an image is with markdown like this:

![Alt Text Goes Here](../assets/branding/header.webp)

You can also use html, but you might need to specify the maximum allowed width so it doesn't clip outside of the page if the base size is too big:

<img src="../assets/branding/header.webp" alt="Alt Text Goes Here" style="max-width:100%;" class="no-lightbox">

Images will by default be clickable to open in what's called a lightbox, no matter which method you add them with. If you want this to NOT be the case, use the html method and add the class `no-lightbox`, as with the example above.

Videos have to be added with html. The `controls` tag shows the controls, `loop` makes it loop, and `autoplay` makes it autoplay (as long as there's no audio track, or the video is `muted` by default). This video has all those tags.
<video src="../assets/misc/dingus_example_video.webm" type="video/webm" controls autoplay muted loop style="max-width:100%;"></video>


<!-- AUTHORS -->

# Authors
Each page can have authors listed from the `authors.yaml` database located in `blendwalker/_data`. You add them at the top of each page, and then they'll show up at the bottom by default. Each author must be specified with a unique `key`, and can optionally have a `role` to further clarify what they worked on.  
You can also use the Authors section as something else, like re-naming it by specifying an `authors_title`.  
`authors_id` sets the ID of the `<div>` element the authors are in, so you can make [links that jump directly to that section](#cool-authors).  
Clicking on an Author will take you to their entry in the [About Us](./about_us) page.


<!-- LINKS -->

# Links
Links are pretty neat and really easy.  
[Here's a link to an external website](https://http.cat/)  
If you want to re-use [rickroll] the same link in [rickroll] multiple places you [rickroll] can do it like [rickroll] this!  
Here's how to link to a [specific header](#text)  
Here's how to link to a [specific header on another page](./contributing#make-something)  
It's important to note that you shouldn't include the file extension of pages you link to, because while they might me `.md` now they'll be converted to `.html` later.

[rickroll]: https://www.youtube.com/watch?v=dQw4w9WgXcQ

Please also note that links to assets (not websites) have to be relative to the current file.  
For example, to link to a page next to this one in the folder structure like `contributing.md`, the link should start with `./` to designate it's in the same folder as this file.  
To link to a page in the assets folder, use `../assets/`, for example `../assets/branding/header.webp`. Going from this file in the `docs` directory, `../` takes us out into the root `blendwalker` folder, then from there we can navigate like usual. Into the assets folder, then the branding folder, then specifying the file.



[Just The Docs]: https://just-the-docs.github.io/just-the-docs/