+++
author = "Jatin"
cover = "img/hello.jpg"
date = 2021-02-05T00:00:00Z
description = "How to deploy a jamstack site with hugo and netlify"
draft = true
title = "Using Jamstack"

+++
# Our plan!

We'll use three things for our site:

* Jamstack
* [Netlify](https://netlify.com)
* A custom domain (optional)

We don't need to go into much detail, this tutorial is going to be simple and effective. We'll be using [Hugo](https://gohugo.io) as our static site generator here. So let's understand the basics first and feel free to leave the intro.

## What the heck is jamstack!?

Jamstack is an acronym for Javascript, API and markdown.

* **Javascript** is the language in which most static site generator architecture are written. So what's this static site generator now. It's just a site making tool, makes our work simple.
* **APIs** are **A**pplication **P**rogram **I**nterface. To make it simple, it just allows our code to talk to other code.
* **Markdown** This is simply the new generation of HTML which is simple, fast and good for us.

# Let's Get to Work now.

## Installing Hugo

We'll be using Hugo, since it is fast, simple and yeah, boring (so that you don't go out of your way editing the source, which makes our work easier) First we need to install Hugo for our computer system. For details about installing Hugo, you can read the [official documentation](https://gohugo.io/getting-started/installing/ "docs").

Here's the gist of it.

### For Windows

For windows, you just need to run these commands in Command Prompt

        choco install hugo -confirm

This installs Hugo in the path, but sometimes you need an extended version for SCSS/CSS interconversion, so I recommend installing the 'extended' version

        choco install hugo-extended -confirm

The extended version is better if you are making a modern day site.

### For Linux

For Linux, you can use the pre installed package manager for example, _apt_ for Debian and Ubuntu, and _zypper_ for OpenSuse etc.

To install it manually, you can download it from the [official Hugo repo](https://github.com/gohugoio/hugo/releases "githubrepo") on github and then use the following commands:

    	tar -xvzf ~/Downloads/*your downloaded tarball*

And now we have to move this file to the bin directory, and for this you will need superuser privileges.

    	sudo mv ~/Downloads/*the directory* /usr/local/bin

And that's it, now you have Hugo up and running, check this by running the _hugo version_ command.

## Making a hugo site.

Now, you can start making a site. To do this, just type this command

        hugo new site <site-name>

When you run this command, a new directory with name _<site name>_ will be created so just get into the directory with the command

 **_cd <site-name>_**

Here's what is should look like

![](/uploads/screenshot-2021-02-06-180611.png)

Now we have to get themes. You can get a lot of themes from all around the internet and for this purpose Hugo has a webpage too! Just go to [https://themes.gohugo.io/](https://themes.gohugo.io/ "https://themes.gohugo.io/")
  
  <p style="text-align: center"> This has to be a centred Text </p>