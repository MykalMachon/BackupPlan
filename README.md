# Backup Plan
my data backup plan 💾🔃

## Why have a personal backup plan?
I don't know about you, but I have a lot of data: photos, university course work, books, source code, etc, etc, etc. In the past, I would just throw this data wherever it best fit (google photos, google drive, github, etc) and sort of *depended* on the fact that everything would be safe as is! 

Then, I started to have things like this happen: 
- I lost ~450GB of RAW photos that I was storing on an external hard drive when I moved.
- Google Photos downgraded lots of my photos to "high quality" (hot tip: they're not very high quality) when I ran out of Google Drive space. 
-  I lost the source code for a significant research project I did in univeristy when a classmate deleted the repo. 

Ouch... 

This data loss could probably have been avoided if I would have been a little more intentional in how I managed my data. Since then, I've invested in a NAS, experimented a bunch, and am now in the process of putting together a personal backup plan 

### Everyone's data is different
Another thing I think is important about having a bit of an individual data backup plan, is that everyone's data is different! 

For example: I have source code on GitHub that I want to backup, which requires some pretty specific tools. Others might have a large bluray collection that they want to backup and have access to. naturally their backup solution would end up looking quite different than mine. 

## Tools 

### Unraid NAS Server
I have an Unraid NAS Server that I use as my primary backup location. It holds *most* of my important files, and has a bunch of nerdy features that let me experiment with virtualization and docker. 
 
The server has 4TB of effective storage set up in raid 1 (2 x 4TB drives), but I have room to upgrade to 8TB if I ever need to.  

### Locally Hosted Apps
These tools are all hosted on my local Unraid Server. 

- [x] **RClone**: for syncing files on my Unraid server to cloud backup locations
- [x] **NextCloud**: for remote access to my photos, documents, and other data. Think of NextCloud like a personal Google Drive.
- [x]  **GitHub Backup**: A simple app that does a nightly sync of all my code on github to my unraid server.
- [x] **Trillium**: A personal knowledge base. I use this to keep daily work notes, meeting notes, and general information / documentation. Think of Trillium like a personal Notion. 
- [x] **Home Assistant**: for managing home automation devices and NFC tags. 
- [x] **NGINX Reverse Proxy**: A simple reverse proxy gui. Makes my services available from the internet. 

### Cloud Components
While I try to keep as much as I can local, there are some tools that are just better in the cloud. 

- [x] Cloudflare: DNS management and proxy. They rock
- [x] BackBlaze B2: very affordable cloud based backup solution that I push my important files to nightly

## General Strategy

WIP: this is going to be an explanation of my backup-plan, inspired by [Jeff Geerling's Backup plan video](https://www.youtube.com/watch?v=S0KZ5iXTkzg)
