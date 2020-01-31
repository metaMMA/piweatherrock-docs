---
title: "Contribution Guidelines"
linkTitle: "Contribution Guidelines"
weight: 10
description: >
  How to contribute to the docs
---

I use [Hugo](https://gohugo.io/) to format and generate this website, the
[Docsy](https://github.com/google/docsy) theme for styling and site structure,
and [Netlify](https://www.netlify.com/) to manage the deployment of the site.
Hugo is an open-source static site generator that provides templates,
a standard directory structure in which to organize content, and a website generation
engine. Pages can be written in Markdown or HTML (or both if you want), and Hugo
will convert them into a website like this one.

All submissions, including submissions by project members, must come via a GitHub
pull requests. Consult GitHub's [Proposing changes to your work with pull requests](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests)
docs for more information.

## Quick start with Netlify

Here's a quick guide to updating the docs. It assumes you're familiar with the
GitHub workflow and you're happy to use the automated preview of your doc
updates:

1. Fork the [PiWeatherRock Docs repo](https://github.com/genebean/piweatherrock-docs) on GitHub.
2. Create a new branch for your work
3. Make your changes and send a pull request (PR).
4. If you're not yet ready for a review, add "WIP" to the PR name to indicate
   it's a work in progress. (**Don't** add the Hugo property
   "draft = true" to the page front matter, because that prevents the
   auto-deployment of the content preview described in the next point.)
5. Wait for the automated PR workflow to do some checks. When it's ready,
   you should see a comment like this: **deploy/netlify — Deploy preview ready!**
6. Click **Details** to the right of "Deploy preview ready" to see a preview
   of your updates.
7. Continue updating your doc and pushing your changes until you're happy with
   the content.
8. When you're ready for a review, add a comment to the PR, and remove any
   "WIP" markers.

## Updating a single page

If you've just spotted something you'd like to change while using the docs, Docsy has a shortcut for you:

1. Click **Edit this page** in the top right hand corner of the page.
2. If you don't already have an up to date fork of the project repo, you are prompted to get one - click **Fork this repository and propose changes** or **Update your Fork** to get an up to date version of the project to edit. The appropriate page in your fork is displayed in edit mode.
3. Follow the rest of the [Quick start with Netlify](#quick-start-with-netlify) process above to make, preview, and propose your changes.

## Previewing your changes locally

If you want to run your own local Hugo server to preview your changes as you work:

1. Follow the instructions in Docsy's [Getting started](https://www.docsy.dev/docs/getting-started/) guide to install Hugo and any other tools you need. You'll need at least **Hugo version 0.63.1** (we recommend using the most recent available version), and it must be the **extended** version, which supports SCSS (the version installed by Homebrew on macOS is the right version).
2. Fork the [PiWeatherRock Docs repo](https://github.com/genebean/piweatherrock-docs) repo as talked about above and then create a local copy using [`git clone --recurse-submodules`](https://www.git-scm.com/docs/git-clone#Documentation/git-clone.txt---recurse-submodulesltpathspec). Be sure to use `--recurse-submodules` or you won’t pull down some of the code you need to generate a working site.

    ```bash
    git clone --recurse-submodules --depth 1 \
    https://github.com/<your username>/piweatherrock-docs.git
    ```

3. Run `hugo server` from inside the piweatherrock-docs folder. By default your site will be available at http://localhost:1313/. Now that you're serving your site locally, Hugo will watch for changes to the content and automatically refresh your site.
4. Continue with the usual GitHub workflow described above to edit files, commit them, push the changes up to your fork, and create a pull request.

## Creating an issue

If you've found a problem in the docs, but you're not sure how to fix it yourself, please create an issue in the [PiWeatherRock Docs repo](https://github.com/genebean/piweatherrock-docs/issues). You can also create an issue about a specific page by clicking the **Create Issue** button in the top right hand corner of the page.

## Useful resources

* [Docsy user guide](https://www.docsy.dev/docs/): All about Docsy, including how it manages navigation, look and feel, and multi-language support.
* [Hugo documentation](https://gohugo.io/documentation/): Comprehensive reference for Hugo.
* [Github Hello World!](https://guides.github.com/activities/hello-world/): A basic introduction to GitHub concepts and workflow.
