
# Get Started

## Requisites

* [Git](https://www.atlassian.com/git/tutorials/install-git#linux)
* [Docker](https://docs.docker.com/engine/installation/)
* [Docker-Compose](https://docs.docker.com/compose/install/#install-compose)

## Forking

Fork this repository.

## Clone

```
git clone git@github.com:YOUR_GITHUB_USERNAME/mobile.frontendlabs.io.git
```

```
cd mobile.frontendlabs.io
```

## Update submodules (only the first time)

```
git submodule update --init --recursive
```

## Run

```
docker-compose up
```

## Open your browser

```
http://localhost:1313/
```

## Creating a new post

This command creates a markdown file on the following path: `source/content/posts/`.

> _This only works when your container is up and running_.

### Create a new post

```
make newpost name=post_name
```

### Change status

Open your new file `source/content/posts/post_name.md` with an editor and change the value of `draft: true` to `draft: false`, and write some of markdown like this:

```
---
title: "Post_name"
date: 2017-10-06T22:26:57Z
draft: false
---

## Subtitle

paragraph paragraph paragraph paragraph.
```

Save your changes.

## Open your browser

```
http://localhost:1313/
```

# Extras

## Add another theme

```
git submodule add git@github.com:GITHUB_ACCOUNT/hugo-THEME_NAME.git source/themes/THEME_NAME
```

## Creating a custom post from Docker-compose

```
docker-compose exec hugo sh -c "hugo new posts/post_name.md"
```

# Contrib
