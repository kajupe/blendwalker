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

- TOC
{:toc}
<!-- Here's how to add a comment -->
<!--
It can span multiple lines! Anything between those two tags will be ignored, and is only for taking notes essentially.
That thing up there above these comments btw is how to add a table of contents (TOC)
It automatically generates a list of all the headers in the page and makes links to them.
You'll notice that the first header (#Example Page) has a little tag below it { .no_toc }, which excludes it from the toc.
-->


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

![Alt Text Goes Here](../assets/branding/header.png)

You can also use html, but you might need to specify the maximum allowed width so it doesn't clip outside of the page:

<img src="../assets/branding/header.png" alt="Alt Text Goes Here" style="max-width:100%;">

Videos have to be added with html. The `controls` tag shows the controls, `loop` makes it loop, and `autoplay` makes it autoplay (as long as there's no audio track, or the video is `muted` by default). This video has all those tags.
<video src="../assets/misc/dingus_example_video.webm" type="video/webm" controls autoplay muted loop style="max-width:100%;"></video>


<!-- AUTHORS -->

# Authors
Each page can have authors listed from the `authors.yaml` database located in `blender-xiv/_data`. You add them at the top of each page, and then they'll show up at the bottom by default. Each author must be specified with a unique `key`, and can optionally have a `role` to further clarify what they worked on.  
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

[rickroll]: https://www.youtube.com/watch?v=dQw4w9WgXcQ

Please note that links to assets (not websites) have to be relative to the current file.  
For example, to link to a page next to this one in the folder structure like `contributing.md`, the link should start with `./` to designate it's in the same folder as this file.  
To link to a page in the assets folder, use `../assets/`, for example `../assets/branding/header.png`. Going from this file in the `docs` directory, `../` takes us out into the root `blender-xiv` folder, then from there we can navigate like usual. Into the assets folder, then the branding folder, then specifying the file.
