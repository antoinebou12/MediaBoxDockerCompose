# MediaBoxDockerCompose
Sonarr | Radarr | Jackett | NZBGet | Deluge | Plex | Jellyfin | Ombi | Tautulli | Netdata | Dashmachine | FileBrowser | Lidarr

TV shows, movies, music download, sort, with the desired quality and subtitles ready to watch, in a beautiful media player. All automated.

inspired by https://github.com/sebgl/htpc-download-box#setup-sonarr

- Administration tools 
   - Netdata
     - `http://10.0.0.4:19999`
   - FileBrowser
     - `http://10.0.0.4:8999`

- Torrenting tools
  - Deluge
    - `http://10.0.0.4:8112`
    password: deluge
  - NZBGet
    - `http://10.0.0.4:6387`
    - username: nzbget
    - password: tegbzn6789
  - Jackett
    - `http://10.0.0.4:9117`

- Automatic Downloader
  - Sonarr: Tv Shows 
    - `http://10.0.0.4:8989`
  - Radarr: Movies
    - `http://10.0.0.4:7878`
  - Lidarr: Music
    - `http://10.0.0.4:8686`
  - Bazarr: subtitle
    - `http://10.0.0.4:6767`

- Plex And Media 
  - Plex
    - `http://10.0.0.4:32400`
  - Ombi
    - `http://10.0.0.4:3579`
  - Tautulli
    - `http://10.0.0.4:8063`
  - Jellyfin
    - `http://10.0.0.4:8096`
  - Couchpotato
    - `http://10.0.0.4:5050`

- Web portal
  - Dashmachine
    - `http://10.0.0.4:5000`
