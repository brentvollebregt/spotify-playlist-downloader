# Spotify Playlist Downloader
Download Spotify playlists to mp3 files that are tagged and given album art. Uses YouTube as an audio source by looking for lyric videos and Spotify to tag and allow the user to choose songs more easily.

# Requirements
* Python (tested with 3.5)
* ffmpeg (described in Installation#4+5)

# Installation
1. Clone this repository. `git clone https://github.com/brentvollebregt/spotify-playlist-downloader.git`
2. cd into the project. `cd spotify-playlist-downloader`
3. Go to [https://developer.spotify.com/my-applications](https://developer.spotify.com/my-applications) and create an app to get a client_id and client_secret key pair
4. Put these keys in settings.json
5. Go to [http://ffmpeg.zeranoe.com/builds/](http://ffmpeg.zeranoe.com/builds/) and download ffmpeg.
6. Extract the files and copy ffmpeg.exe, ffplay.exe and ffprobe.exe from the /bin folder to the location of spotify_album_downloader.py (you can also put these in a location that is reference by the PATH variable)

# Usage
1. Get the URI of a Spotify playlist by clicking the three dots at the top to show then menu and click share. In this sub-menu, click "Copy Spotify URI"; this will copy the URI to your clipboard.
2. Run spotify_album_downloader.py and insert your Spotify URI, then hit enter.
3. Files will be saved to /output/ in the current working directory.
