PNWPHP Website
==============

This repository contains (almost) everything that makes up
[pnwphp.com](https://pnwphp.com).

Powered by [Sculpin](https://github.com/sculpin/sculpin). =)

Install Tools
-------------

### Install SASS and Bower

    gem install sass
    npm install bower
    
### Install Sculpin

See [Download and Install Sculpin](https://sculpin.io/getstarted/#download-and-install-sculpin) from the Sculpin "Get Started" guide.

    curl -O https://download.sculpin.io/sculpin.phar
    chmod +x sculpin.phar
    mv sculpin.phar ~/bin/sculpin
    
Note: Make sure `~/bin` is in your path.

Build
-----

### Run SASS

    sass --watch sass/main.scss:source/assets/css/main.css -I .

### Run Sculpin

    sculpin install
    sculpin generate --watch --server

Your local copy of [pnwphp.com](https://pnwphp.com) is now accessible at `http://localhost:8000/`.

Notes
-----

This was setup to use NPM to install Bower locally. I am not 100% certain how to
best get SASS into the mix so I was just using SASS locally.It would probably be
a good idea to get this all built into one system so possibly getting NPM to
install SASS so that it can be run locally without having it be required to be
installed globally?
