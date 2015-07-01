<<<<<<< HEAD:README.md
ImgDown
=======

I made this program as a practice to learn ruby. What this program does is to
recursively search a HTML-document for links and images a extract their source
and pointer. Then with regular expression you can choose what of those you want
to download.

Installation
------------
If you haven't Ruby v1.9.3 installed please install it first. Please consult
the official documentation on 
[how to do that](https://www.ruby-lang.org/en/documentation/installation/).

Clone this repo and then install its dependencies by running this in the
terminal:
`sudo gem install -g`

If you want to make a system wide installation then you can run if you want to:
`cp imgdown /usr/local/bin/`

Usage
-----

To get all links and pictures from a webpage, just type:
./imgdown --link http://link/to/webpage

This works for https links as well.
./imgdown --link https://link/to/webpage

To specify with regex, type:
./imgdown --link http://link/to/weboage --reg-ex "catpictures[0-9]+\.jpe?g"

Found a range of picture you want to download? Download with:
./imgdown --link http://link/to/weboage --reg-ex "catpictures[0-9]+\.jpe?g" --download

You might want to specify location.. 
./imgdown --link http://link/to/weboage --reg-ex "catpictures[0-9]+\.jpe?g" --download --destination "~/mycatpictures"

The website didn't want you to download your catpictures? Hehehe..
./imgdown --link http://link/to/weboage --reg-ex "catpictures[0-9]+\.jpe?g" --download --destination "~/mycatpictures" --user-agent "Catfox v.1337"

You're a person who forgets a lot?
./imgdown --help

