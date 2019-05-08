# Rollout
Possibly the fastest one-page GitHub pages template to deploy.

![Logo](assets/logo.svg)

## Overview
Rollout is a single-page GitHub pages template thing that literally shows a logo, links to your project and profile, and loads your project's readme file into the page (rendering the markdown as it does so). This makes it really, really straightforward to roll out a basic GitHub pages site straight away.

## Configuration
Rollout powers its own [GitHub pages site](https://lambdacasserole.github.io/rollout/). To configure it:

1. Clone this repo.
2. Open up the `/docs` folder.
3. Change the logo at `/docs/svg/logo.svg` to your own.
4. Open up `/docs/index.html` in your favorite text editor.
    * Change the contents of the `title` tag.
    * Change the contents of the `meta` tags with names `description` and `author`.
    * Change the `username` and `repo` JavaScript `const` declarations to your GitHub username (or organization name) and repository name respectively.
5. Deploy it as your pages project, you're done!

If you're not familiar with setting up GitHub pages, [this is the article for you](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages).

### Specifics
More specifically, you need to find these lines:

```html
<title>Rollout - Very fast GitHub pages deployment</title>
<meta name="description" content="Possibly the fastest one-page GitHub pages template to deploy.">
<meta name="author" content="Saul Johnson">
```

Replace the title, description and author with your own values. Now, find these lines:

```js
// Configure the page here.
const username = "lambdacasserole";
const repo = "rollout";
```

Change the value of `username` to your to your GitHub username (or organization name) and `repo` to your repository name. All default values above are for this repository.

## License
This software is public domain, go forth and use it. The same can't be said for any third-party libraries loaded remotely (this project does use [jQuery](https://jquery.com/), [Bootstrap](https://getbootstrap.com/) etc. for example).

Also, by default, "Powered by Rollout" appears in the bottom right-hand corner of the page. You don't have to leave this there, get rid of it if you like, though linking back is appreciated.

## Acknowledgements
I'd like to thank the following people for their contributions:

* The [Showdown](http://showdownjs.com/) JavaScript markdown rendering library.
* The [Bootswatch](https://bootswatch.com/) project. Awesome, free Bootstrap themes over there.
* Yannick Croissant and Kath for the AJAX loader icon generator here: [http://www.ajaxload.info/](http://www.ajaxload.info/)
* Michael Hagemann for the font [Wild Ride](https://www.1001fonts.com/wild-ride-font.html) which is used in the logo.
* The SRI hash generator service [here](https://www.srihash.org/) by [Mozilla](https://github.com/mozilla), which is [open source](https://github.com/mozilla/srihash.org).
