# cply-php

Search lyrics and copy them automatically from the terminal

## Requirements

UNIX-only: Linux, BSD, MacOS

This version is written in PHP and it requires PHP and Composer and a unix system, the song selector of [Climax](https://github.com/tucnak/climax) only works on Unix systems. Tested on Ubuntu (elementaryOS) but should work on others aswell.

It uses my [php clipboard helper](https://github.com/asvvvad/dollaapp-clipboard-php/) which requires `xclip` or `xsel` on Linux and `pbcopy` and `pbpaste` on Darwin

## Install

First, create client id, client secret and token from: https://genius.com/api-clients 

Then clone this repository and install dependencies using:
```bash
git clone https://github.com/asvvvad/cply-php
cd cply-php
composer install
```
After that, edit [cply](cply#L12-L14) with the keys at the begining of the file

Now you can run it using `./cply`

To install it to the system it requires root you can use:
```bash
cd ..
sudo mv cply-php /usr/local/
sudo ln -sf /usr/local/cply-php/cply /usr/local/bin
sudo chmod +x /usr/local/bin/cply
```

## Usage:
[![asciicast](https://asciinema.org/a/MAxxbsticff0vDwLbioaV1wI4.svg)](https://asciinema.org/a/MAxxbsticff0vDwLbioaV1wI4)
