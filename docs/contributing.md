---
title: Contributing
layout: default
nav_order: 9990
authors:
  - key: kaj
  - key: fioh
authors_title: Project Managers
authors_id: project-managers
---

# Contributing
This page is built on community knowledge, and will continue to grow. Do you have anything to share with your fellow creators?

## Quick Contribution
If you want to very quickly just write a guide or suggest a resource and don't want to go through the trouble of learning how to work with Github or build the website locally, don't worry! You can send your guide or suggestion as a [feature request on github] or directly to a [project manager] and it will be looked at. We can't guarantee that it will be added, but the odds are much higher if you follow these guidelines:

### For Resources:
* **Ensure the resource does not seem malicious.**  
If the website looks sketchy, like if it doesn't have any information about who's behind it, it likely won't be accepted
* **Ensure the resource offers high-quality assets.**  
Not *everything* has to be high quality, as is often the case with resource sites where users can submit their own things, but there should be *some* good stuff available.
* **Ensure the resource actually works.**  
Have you tried downloading something? Did it actually work, and you got the file you wanted? Great!
* **Tell us *why* you think this resource should be added.**  
Don't just throw a link at us and call it a day. Tell us about why you like using this resource! We'll take that into consideration.

### For Guides:
* **Ensure it's written well.**  
Try to have good grammar and flow in your writing. Add headers and line-breaks. Your guide shouldn't just be one big block of text.  
One thing to note about line breaks when writing markdown is that one regular line break does nothing. An empty line between two lines starts a new paragraph. A regular line break can be done by adding two spaces at the end of the previous line.
* **Ensure it's informational and uses polite language.**  
It doesn't have to be super formal but don't write something like "Yeah, you'd be pretty stupid to not know this already." or whatever. A guide should provide clear information.

## Detailed Contribution
If you want to make larger changes you may want to have a local copy of the page to work on. This would let you see changes on the page before submitting them to the public. This guide on how to do all that is aimed at newcommers to git, if you're more experienced you'll notice that this isn't the only way of doing it, but it's what we'd suggest new users do.

### Install GitHub Desktop and Ruby
For a local copy of the page you'll need to clone the repository. You'll use [GitHub Desktop] to do this. Then to actually run it you need [Ruby] (which is a programming language) (install it and the develoment kit).

### Set-up
In GitHub Desktop, add a new repository by cloning [the blendwalker repository]. This will copy the entire project into a folder on your computer, by default in a `User > Documents > GitHub` folder. If you go to `Repository > Show in Explorer` it will open the folder.

Once in the folder, right click on some empty space and click `Open in Terminal`. Then, assuming you have Ruby installed correctly, run `bundle install`.  
That should install a bunch of stuff. Then run `bundle exec jekyll serve` to host the page locally. It will say which ip it's being hosted on, by default it should be [http://127.0.0.1:4000/](http://127.0.0.1:4000/). Then any time you edit a file, such as adding or editing a page located in the `docs` directory, just reload the page and you'll see the changes.

### Make Something
Some things to keep in mind when you make a contribution:  
* **Optimize Files**  
Your images should ***always*** be smaller than a megabyte, and usually way smaller than that! Longer videos are the only thing that should ever end up over a megabyte, but try to compress as much as possible while still keeping images legible. Try using formats like .webp and .jpg, those tend to be pretty small. For videos, try to use AV1 or H.265 encoding, with Opus as the audio codec. As long as it's small, it's fine.  
* **Name Files Well**  
You should name files using underscores_instead_of_spaces_like_this, and the names should be descriptive. Ideally they should also be prefixed with something that relate to where they end up. For example if you're adding five images for your hypothetical guide on using mocap data, prefix them with "mocap_yourname", so the full name is something like "mocap_yourname_description". That way they'll end up next to each other in the file order!  
* **You can be Fancy**  
This page is based on [Just The Docs] and lets us do a lot of fun things if we want, outside of regular markdown documents. You can write whatever html and css and javascript you want really. If you have an idea for something you want laid out in a specific way, it's probably possible, and those languages have a lot of resources for learning. The [Just The Docs] page also has a lot of information on how to make things.    
* **Look at the Example Page**  
There's an unlisted page you can use as a reference for a bunch of stuff. You can go to it [here](./example_page), but it's most useful to look at as a markdown file, which you can do in the [GitHub repo](https://github.com/kajupe/blendwalker/blob/main/docs/example_page.md)  
* **Add yourself as an Author**  
If you've made something, we want people to know that it was you who did it! You should add yourself as an Author to your page. There's a guide for that in the [example page](./example_page#authors).

### Submit your Changes
Once you're happy with your contribution, give it a Summary / Title in GitHub Desktop as well as a Description. For example the Summary could be "Added a Guide about Mocap Retargetting" and the Description could be anything you want really, relevant information about your contribution. It's mostly for you. Then click `Commit to main`. Then you can click `Push origin` in the new big blue button on the right, to upload it to GitHub.  
By this point you have an entirely separate version of the page with your changes. Now you just need to request for us to look at it and add it to the public page with a pull request. To do this, go to your repository on GitHub. You can see all your repositories at `https://github.com/your-username?tab=repositories`. Near the top of that page it should say "This branch is X commits ahead of kajupe/blendwalker:main". To the right of that is a button that says `Contribute`. Click that, then `Open pull request`. Give it a title and description here as well, and click `Create pull request`. We will then be notified that you want to submit a change and can either chose to accept it or request that you make changes to it first.


[the blendwalker repository]: https://github.com/kajupe/blendwalker/
[feature request on github]: https://github.com/kajupe/blendwalker/issues
[project manager]: #project-managers
[GitHub Desktop]: https://desktop.github.com/download/
[Ruby]: https://rubyinstaller.org/
[Just The Docs]: https://just-the-docs.github.io/just-the-docs/