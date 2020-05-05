# MediaBoxDockerCompose
Sonarr | Radarr | Jackett | NZBGet | Deluge | Plex | Jellyfin | Ombi | Tautulli | Netdata | Dashmachine | FileBrowser | Lidarr | Samba | Wireguard-as

TV shows, movies, music download, sort, with the desired quality and subtitles ready to watch, in a beautiful media player. All automated.

inspired by https://github.com/sebgl/htpc-download-box#setup-sonarr

- Administration tools 
   - Netdata
     - `http://<your_ip>:19999`
   - FileBrowser
     - `http://<your_ip>:8999`
     - username: admin
     - password: admin
     - before docker-compose up create file in the ${ROOT}/config/filebrowser/database.db
   - Samba
      - `http://<your_ip>/Mount`
   - Wireguard
      - `http://<your_ip>;8000`

- Torrenting tools
  - Deluge
    - `http://<your_ip>:8112`
    - password: deluge
    - Extra: use the auth
  - NZBGet
    - `http://<your_ip>:6387`
    - username: nzbget
    - password: tegbzn6789
  - NBZHydra:
     - `http://<your_ip>:5076`
  - Jackett
    - `http://<your_ip>:9117`

- Automatic Downloader
  - Sonarr: Tv Shows 
    - `http://<your_ip>:8989`
  - Radarr: Movies
    - `http://<your_ip>:7878`
  - Lidarr: Music
    - `http://<your_ip>:8686`
  - Bazarr: subtitle
    - `http://<your_ip>:6767`

- Plex And Media 
  - Plex
    - `http://<your_ip>:32400`
  - Ombi
    - `http://<your_ip>:3579`
  - Tautulli
    - `http://<your_ip>:8063`
  - Jellyfin
    - `http://<your_ip>:8096`
  - Couchpotato
    - `http://<your_ip>:5050`

- Web portal
  - Dashmachine
    - `http://<your_ip>:5000`
    - use the dashmachine.config.ini in [Setting]
