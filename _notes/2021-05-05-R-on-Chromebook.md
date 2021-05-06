---
title: Installing R on a chromebook
layout: default
---

Before beginning this, you need to have enabled the Linux shell.

1. Pick a mirror, (I chose: http://ftp.ussg.iu.edu/CRAN/)
2. Acccording to the docs, add this repo to install a recent version of R: 
`deb http://cloud.r-project.org/bin/linux/debian buster-cran40/` 
to the file `/etc/apt/sources.list` on your computer.
3. `sudo apt update && sudo apt upgrade`
4. `sudo apt install r-base r-base-dev`

### Install cryptography packages

Following along the notes from [a cryptography class](https://djhunter.github.io/cryptography/slides/01intro_crypto.html#/shift-cipher-implemented-in-r), 
you might want to install some helpful packages. These might have OS pre-requisites, like `lib gmp`:

    sudo apt-get install libgmp3-dev
