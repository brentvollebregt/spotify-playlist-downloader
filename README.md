# spotify-playlist-downloader
Downloads Spotify playlists to mp3 files that are then tagged and given album art.

# Requirements
* Python (tested with 3.5)
* mutagen (pip install mutagen)
* youtube_dl (pip install youtube_dl)
* BeautifulSoup4 (pip install beautifulsoup4)
Note: Spotipy is also required but I have included it in this repository. Gathered from [https://github.com/plamere/spotipy](https://github.com/plamere/spotipy).

# Installation
1. Make sure requirements are installed
2. Go to [https://developer.spotify.com/my-applications](https://developer.spotify.com/my-applications) and create an app to get a client_id and client_secret key pair
3. Put these keys in settings.json
4. Go to [http://ffmpeg.zeranoe.com/builds/](http://ffmpeg.zeranoe.com/builds/) and download ffmpeg.
5. Extract the files and copy ffmpeg.exe, ffplay.exe abd ffprobe.exe from the /bin folder to the location of spotify_album_downloader.py

# Usage
1. Get the URI of a spotify playlist by sharing it and clicking URI on the far right. This will copy the URI to your clipboard.
2. Run spotify_album_downloader.py and insert your Spotify URI, then hit enter.
3. Files will be saved to /output/ in the cwd.

# Notes
You do what you want with this project, I will not be held liable for any troubles you may face from this