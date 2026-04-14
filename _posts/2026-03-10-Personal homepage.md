---
title: My own page in the web
date: 2026-03-10
tags: []
toc: false
comments: false
description: Using Jekyll and GitHub pages to bring this blog to you
image:
    path: /media/blog_page/jekyll.webp
    alt: logo of jekyll ssg
---

Since I am making this page right now in order for you to read this, I figured I might as well describe how I am making it. It is a very standard process, and for good reason---I can only recommend it.

As shown in this post's title image, I am using the static site generator **Jekyll**. When using Jekyll to create a static webpage, it is very common to start with a _Jekyll theme_, of which there are many.
I found that the best place to look for themes is in the [jekyll-theme topic on GitHub](https://github.com/topics/jekyll-theme). However, other indexes of Jekyll themes exist as well.

Once I had chosen the [**Chirpy theme**](https://github.com/cotes2020/jekyll-theme-chirpy)---one of GitHub's most popular---, I simply followed Chirpy's [Getting Started guide](https://chirpy.cotes.page/posts/getting-started/).
First, I used Chirpy as a template GitHub repository, which gave me all the necessary files to start. Since the Chirpy theme is quite sophisticated, this comes with a devcontainer. Thus, development is extremely straightforward and does not require any manual installations when using an IDE which supports devcontainers, such as [Zed](https://zed.dev/) or [neovim](https://codeberg.org/esensar/nvim-dev-container) 😁. Especially convenient if you do not otherwise need Ruby tool chains, since Jekyll is built in Ruby. 

From here, I could already launch the empty Chirpy theme using 
```terminal
$ bundle exec jekyll serve
```
The site is then found at port 4000.

Before filling in the pages' contents, I slightly modified the template next. To do so, I located the theme's source files, which had been pulled to my machine using 
```terminal
$ bundle show chirpy
```
This returns the path, in my case: `/usr/local/rvm/gems/default/gems/jekyll-theme-chirpy-7.5.0`{: .filepath}

Doing so is necessary because these source files, which are drawn from the theme's rubygem, are not part of the template repository but are instead used during deployment to build the site. In order to modify the look of the site, then, you can _copy_ any file from that directory to your base project directory while maintaining the subdirectory structure, e.g., `[template path]/_layouts/default.html`{: .filepath} to `[project path]/_layouts/default.html`{: .filepath}. From here, modify the file in your project directory. When the site is generated during deployment, all files present in the project space will overwrite the template's source files. This goes for HTML and SCSS alike. 

With the site looking as I wanted it to, added content is very simple (this is the point of SSGs after all). All pages and posts are written in Markdown and placed in the pre-made folders, as specified by the Chirpy template. 
Running `bundle exec jekyll serve` then compiles all Markdown files into the static website. I found that hot reloading on file change was not working reliably, but keyboard-interrupting the local server and recompiling works just fine. For me, the site generation typically took between 5 and 10 seconds every time. 

I set my copy of the Chirpy template repository to private when creating it, in order to back up my development changes and share them between devices before making them presentable. For deployment, I copied the Chirpy template again, only this time as a public repository. This is necessary to deploy from **GitHub Pages** (given you do not have a paid GitHub plan). I could now copy my private changes to the public repository. The Chirpy theme includes all necessary workflow configurations to generate and deploy the site. Thus, setting the GitHub Pages deployment source to GitHub Actions will allow for an updated deployment whenever changes are pushed to the repository and trigger the pipeline.

![Desktop View](/media/blog_page/porkbun.webp){: width="972" height="589" .w-25 .right}

Finally, I purchased this custom domain at Porkbun. The setup does work entirely without a custom domain and is then reachable at `[GH user name].github.io`. Setting a custom domain is mostly just polish. To set it up, I added the appropriate A and AAAA records pointing to GitHub's servers (as specified in GitHub Pages's documentation) to my DNS records and linked the domain in the repository settings.

Et voilà! The website is right here where you're viewing it. It is version-controlled, automatically deployed, easy to maintain and expand. All in all, at a cost of $1/month (for the domain name).
