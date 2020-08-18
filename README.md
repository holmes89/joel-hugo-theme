# Joel - Hugo theme
Joel is a simple theme for blogs.

Forked from [Archie Theme](https://github.com/athul/archie)

## Demo

[Check the Demo](https://athul.github.io/archie/) hosted on GitHub Pages :smile: . You can find the source code to that in the `site` branch of this repository

![](/images/theme.png)
![](/images/archie-dark.png)
## Feature
- Google Analytics Script
- Callouts
- Tags
- tl:dr; frontamatter

## Installation
In your Hugo website directory, create a new folder named theme and clone the repo
```bash
$ mkdir themes
$ cd themes
$ git clone https://github.com/holmes89/joel-hugo-theme.git
```
Edit the `config.toml` file with `theme="joel"`
For more information read the official [setup guide](https://gohugo.io/overview/installing/) of Hugo.

## Writing Posts
Create a new `.md` file in the *content/posts* folder
```yml
---
title: Title of the post
description:
date:
tldr: (optional)
draft: true/false (optional)
tags: [tag names] (optional)
---
```

## Credits
Forked from [Archie Theme](https://github.com/athul/archie) and Licensed under MIT License 
Inspired by design of blog.jse.li

----

## Config of the Demo Site

```toml
baseURL = "https://joelholmes.dev
languageCode = "en-us"
title = "Joel Holmes"
theme="joel"
copyright = "© Joel"
# Code Highlight
pygmentsstyle = "monokai"
pygmentscodefences = true
pygmentscodefencesguesssyntax = true

paginate=3 # articles per page

[params]
	mode="auto" # color-mode → light,dark or auto
	featherIconsCDN=true
	subtitle = "Clean [blog theme for Hugo](https://github.com/holmes89/joel-hugo-theme)"

# Social Tags

[[params.social]]
name = "GitHub"
icon = "github"
url = "https://github.com/athul/archie"

[[params.social]]
name = "Twitter"
icon = "twitter"
url = "https://github.com/athulcajay/"

[[params.social]]
name = "GitLab"
icon = "gitlab"
url = "https://gitlab.com/athul/"

# Main menu Items

[[menu.main]]
name = "Home"
url = "/"
weight = 1

[[menu.main]]
name = "All posts"
url = "/posts"
weight = 2

[[menu.main]]
name = "About"
url = "/about"
weight = 3

[[menu.main]]
name = "Tags"
url = "/tags"
weight = 4
```