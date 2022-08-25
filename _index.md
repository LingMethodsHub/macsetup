---
title: "Basic macOS Command Line Setup"
format: 
  html:
    theme: materia
    toc: true
    toc-location: left
author: Josef Fruehwald
date: 2022-8-25
license: CC-BY-SA 4.0
editor: visual
draft: false
weight: 10
---



Fresh out of the box, there are a few bits of configuration you'll need to do to get your macOS computer ready for scientific computing.

1.  Make sure "command line tools" are installed.
2.  Install a package manager.

## Command Line Tools

"Command line tools" are a basic set of programs you run at the command line, that for some reason don't come installed by default on macOS.

The easiest way to install them through the command line in the Terminal app. You can launch Terminal either with spotlight search, or by finding it inside Applications/Utilities.

Once you've launched Terminal, type (or copy+paste) the following command.

``` zsh
xcode-select --install
```

At this point, a window may pop up asking you to confirm that you want to install command line developer tools. Click "Install."

Once installation has completed, you may need to restart Terminal, but every necessary command line program should now be installed.

## Install a package manager

A "package manager" is program that helps you install, configure, and keep up-to-date programs without needing to go visit software websites or download installers. macOS doesn't come with a default package manager, but most people use [homebrew](https://brew.sh/).

To install homebrew, vist [brew.sh](https://brew.sh/) and run the install code on their home page.

Now, when you need to install a piece of software you'll use at the command line, you can just run `brew install` followed by its name (if it has a "formula" available). For example, even though it has a stand-along program, sometimes people want to use [Praat](https://www.fon.hum.uva.nl/praat/) at the command line. We can make praat available at the command line easily with

``` zsh
brew install praat
```
