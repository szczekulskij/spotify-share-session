# spotify-share-session
web application for sharing spotify's queue live w. chat and ai suggested songs

## Conceptual:
### Basic functionality:
* Have a website on which there is a music queue that plays music 
* Have multiple users logged in that can add their songs to the queue

### Extended functionality:
#### backend & frontend:
* Have a chat
* Leave emoji under song functionality
* Enable users to vote on which song to play
* Admin/subadmin/normie priveleges w. different power levels

#### AI:
* AI 'quick' song reccommender - 'based on your **currentely** played song - you should listen to ...'
* AI 'long-term' song reccommender - 'based on the **last 10 songs/30 minutes** - you should try ...'

#### Database:
* Save users login & password (hashed)
* Save users played songs in database to be used for AI reccommender

## Initial Plan:
### Initial blockers:
* API for spotify, we need it to either:
  * Request & recevice a song so we can play it (most likely not possible)
  * Enable our site to handle log in as a user(optimal anyway) & then send our away the music that user requests (if that's possible, then we can also handle logging of other people joining chatroom & enable them searching songs from their fav playlists - otherwise they need to search a song on their spotify -> type it in our webapp - which isn't bad per se, but not optimal)

### Possible blockers workarounds:
* Use youtube API (this one has possibility of playing any video song - like in [Joma Tech Video](https://www.youtube.com/watch?v=OHviieMFY0c&t=95s&ab_channel=JomaTech)
* 





## Tech Stack:
* Backend - java (spring boot)
* Frontend - javascript (react)
* Server - Linux Centos 6/7 running from AWS
* Database - yet to choose (CockroachDB/MySQL)
* AI - yet to choose (pytorch, fastai, gpt-3 or already implemented song-related AIs)
