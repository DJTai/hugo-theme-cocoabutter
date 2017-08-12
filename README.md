# Cocoabutter theme for Hugo

A fork of the [Cocoa theme](https://github.com/nishanths/cocoa-hugo-theme/) with:

* A static home page created with "index.md"
* A "Latest Post" summary on the blog page

TODO:
* Set accent color to be configurable via "config.toml"
* Make links in "header.html" partial update with new top level pages automatically
* Demo site

See README for Cocoa theme [here](https://github.com/nishanths/cocoa-hugo-theme/blob/master/README.md).

## Screenshots

![Index](/exampleSite/cocoabutter-1.jpg)
***
![Blog](/exampleSite/cocoabutter-2.jpg)
***
![Post page](/exampleSite/cocoabutter-3.jpg)
***
![Contact page](/exampleSite/cocoabutter-4.jpg)
***

## Table of Contents

* [Quick start](#quick-start)
* [Usage](#usage)
* [Development](#development)
* [Changelog](#changelog)
* [License](#license)

## Quick start 

From the root of your Hugo site, clone the theme into `themes/cocoabutter` by running:

```sh
# Clone theme into the themes/cocoabutter directory
$ cd themes
$ git clone https://github.com/hivickylai/hugo-theme-cocoabutter.git cocoabutter

# Serve your site and visit localhost:1313 in your browser
$ hugo -t cocoabutter --watch serve

# Generate site files into the public directory
$ hugo -t cocoabutter
```

## Usage

#### config.toml

Please see the sample [`config.toml`](https://github.com/hivickylai/hugo-theme-cocoabutter/blob/master/exampleSite/config.toml)

#### Creating the home page (index.md)

Create your index page in the `content` directory by running:
```
hugo new index.md
```

In the front matter of the file, include `type = "index"` like so:
```
+++
date = "2017-02-08T13:28:26+07:00"
draft = false
title = "Home"
type = "index"
+++
```

#### Creating posts

Posts should generally go under a `content/blog` directory. Typically you would run:

````
hugo new blog/your-new-post.md
````
For posts to appear on your site, you may need `draft = false` in the post's front matter or use the `--buildDrafts` option when building.

#### Creating fixed pages

Fixed pages such as an About page should preferably go under `content/fixed` or be present at the root of the `content` directory.

````
hugo new fixed/about.md
````

## License

Licensed under the MIT License. See the [LICENSE](https://github.com/hivickylai/hugo-theme-cocoabutter/blob/master/LICENSE) file for more details.
