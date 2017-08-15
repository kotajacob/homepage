# homepage
A simple and minimal homepage. Now compatible with WAL and WPG!

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
