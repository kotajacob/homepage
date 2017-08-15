# homepage
A simple and minimal homepage. Now compatible with WAL and WPG!

## About

The homepage is setup giving you a nice clean search bar which
you can easily search your favorite search engine with (by default it's 
duckduckgo)

If you press enter with nothing in the search bar you'll notice a chart of 
hotkeys. Each of the letters can be searched alone to quickly go to the 
associated website.

In addition to just going quickly to those websites you can even search them 
(or in reddits case quickly go to a subreddit) by typing the letter colon then
the search.

For example this will search and goto the WW2 page on wikipedia
wi:World War 2
or go to askreddit
r:askreddit

All of this is easily customized in a simple table in homepage.html

## Usage
### Firefox
Install firefox and then get the extention New Tab Override.

Due to a recent firefox update it is no longer possible for extentions to read 
local files. This means if you want to use this homepage with firefox you need
to host a minimal webserver in the background and then have new tab override 
point to 127.0.0.1 (the address of the local server on your computer)

On linux this is fairly simple.
This is assuming you're using arch, if not substitute the commands and 
directories used in your distro.

pacman -S nginx

sudo chown yourusername:yourusername -R /usr/share/nginx/html

git clone https://github.com/kotajacob/homepage /usr/share/nginx/html

sudo systemctl enable nginx

sudo systemctl start nginx

Then confirm firefox loads the new tab page when you visit http://127.0.0.1/homepage.html

Finally set new tab override to load custom URL with the set focus option enables
make the url the following http://127.0.0.1/homepage.html 

### Chrome/Chromium
Install chrome or chromium and then get the extention New Tab Redirect

clone or download the repo

(maybe move it to a sensible place other than downloads)

open homepage.html with chrome

copy the address and set New Tab Redirect to open that address

## Screenshots

![Blank default setup](https://i.imgur.com/1TNc1vG.png)

![Enter menu](https://i.imgur.com/My6CgaE.png)

![Enter menu](https://i.imgur.com/My6CgaE.png)

![Go to subreddit](https://i.imgur.com/4hpmbYO.png)

![Search github for linux](https://i.imgur.com/GL67ohK.png)

![Search wikipedia for ww2](https://i.imgur.com/LBE6nZT.png)

![A different color scheme](https://i.imgur.com/bboFM5P.png)

![A different color scheme menu](https://i.imgur.com/fUCkn29.png)