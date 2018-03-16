
# Direct Plex Downloader  

## Description / Background
Powershell script to help download items from a plex server.

## Details
Can be used on your own server or on a remote friends server as well.
Requires knowing a few things about the plex server:
1. Plex Token (Either the server owners token, or the token issued to you for accessing a friends server)
2. Plex Server url:port (can be a known ip, the plex.direct url, or a friendly url )
3. Metadata ID of the movie/show you want to download.

A better method of this would be to make this in python and use the plex-api to search for the name of what you want, 
rather than needing the metadata ID, but I'll leave that for someone else.

## Configuration:
* Modify the top of the script and change the 3 variables to your own.
$TOKEN = Either your own token if using for your own server, or the token issued to you for accessing your friends server.
One way to find this is to use the browser and inspect the element and look in the network tab.

* $URL = Url and port of plex server. Can be an IP, plex.direct or friendly url
ie: https://43.134.28.231:32400
ie: https://43-134-28-231.af3e77ad3484fc98113453526hf5433.plex.direct:5280
ie: https://watch.myplexmovies.com

* $PATH = Local path to where the download will save.
ie: c:\temp\plex_downloads\

## How to use
1. Launch the script
2. It will ask for the movie or TV Show Metadata ID.
This can be found on the end of the url in your browser when looking at a movie or TV shows details in plex web.
3. Hit enter, this will start the download and show you a friendly progress bar and ETA.

## Errors
If you get an error it's probably because one of your 3 variables is wrong, or you typed in the wrong metadata ID.
