# Waraki Music Player Katipo Site

Waraki is a standalone local music/mp3 player app, built on top of Katipo. It is a minimal, fully functioning unique and useful cross platform music player.

This repository contains the site package needed to host a waraki instance either via the Waraki app, the [Katipo Browser](https://github.com/mjdave/katipoBrowser), or [katipoHost](https://github.com/mjdave/katipo) command line.

## The files in this repository

### site.tui 

Config file that provides information about the Waraki app/site to Katipo.
### code.tui 
Host-side "backend server" code. It responds to requests, sending playists and songs.
### libraryCrawler.tui 
Tui code that was moved out of code.tui for convenience which does the work of scanning your local directory for music.
### clientSite/ 
Public client-side part of the site. This entire directory is downloaded to the client when they first connect, and the code and resources inside provide the user interface and music playback app experience.