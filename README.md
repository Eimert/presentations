# Presentations [![Build Status](https://travis-ci.org/Eimert/presentations.svg?branch=master)](https://travis-ci.org/Eimert/presentations)

This repository contains my presentations and a travis-ci workflow to create github pages for them.

## View: [https://eimert.github.io/presentations/](https://eimert.github.io/presentations/)

## Presentation writing setup
Want a fast feedback cycle? Run reveal-md using docker.<br>
```
cd presentations/
docker run -it --rm -p 8000:1948 -v $(pwd):/usr/src/app/ containersol/reveal-md:latest
```

## I want this TOO!!!
* copy/paste the .travis.yml and compile.sh to your repo.
* have all the .md presentations in your root folder of your repo
* sign up at https://travis-ci.org/
* create a token at github: https://github.com/settings/tokens (public_repo is the only needed checkmark)
* create an environment with the name GITHUB_TOKEN and as value the token at https://travis-ci.org/username/repo/settings
* After your push to the master branch, your [Project Pages](https://help.github.com/articles/creating-project-pages-using-the-command-line/) site will be available at `http(s)://<username>.github.io/<projectname>`.

Credits: [MansM](https://github.com/MansM/presentations/)<br>
