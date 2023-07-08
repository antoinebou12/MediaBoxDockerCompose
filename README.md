# MediaBoxDockerCompose
Sonarr | Radarr | Jackett | NZBGet | Deluge | Plex | Jellyfin | Ombi | Tautulli | Netdata | Dashmachine | FileBrowser | Lidarr | Samba | Wireguard-as

TV shows, movies, music download, sort, with the desired quality and subtitles ready to watch, in a beautiful media player. All automated.

inspired by https://github.com/sebgl/htpc-download-box#setup-sonarr

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Administration Tools](#administration-tools)
- [Torrenting Tools](#torrenting-tools)
- [Automatic Downloaders](#automatic-downloaders)
- [Media and Player Services](#media-and-player-services)
- [Web Portal](#web-portal)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Install [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/install/) on your system.
2. Clone or download this repository to your system.

## Usage

1. Navigate to the cloned/downloaded directory.
2. Customize the configuration files in the `config` directory to your needs.
3. Run the following command to start the containers:

```bash
docker-compose up -d
```

4. Access the web interfaces for the services by navigating to the URLs mentioned below.

## Administration Tools

- Netdata: http://<your_ip>:19999
- FileBrowser: http://<your_ip>:8999 (username: admin, password: admin)
- Samba: http://<your_ip>/Mount
- Wireguard: http://<your_ip>;8000

## Torrenting Tools

- Deluge: http://<your_ip>:8112 (password: deluge, extra: use auth)
- NZBGet: http://<your_ip>:6387 (username: nzbget, password: tegbzn6789)
- NBZHydra: http://<your_ip>:5076
- Jackett: http://<your_ip>:9117

## Automatic Downloaders

- Sonarr: http://<your_ip>:8989 (TV shows)
- Radarr: http://<your_ip>:7878 (movies)
- Lidarr: http://<your_ip>:8686 (music)
- Bazarr: http://<your_ip>:6767 (subtitles)

## Media and Player Services

- Plex: http://<your_ip>:32400
- Ombi: http://<your_ip>:3579
- Tautulli: http://<your_ip>:8063
- Jellyfin: http://<your_ip>:8096
- Couchpotato: http://<your_ip>:5050

## Web Portal

- Dashmachine: http://<your_ip>:5000 (use the dashmachine.config.ini in [Setting])

## Backup

1. For each service (Sonarr, Radarr, Lidarr, NZBHydra), access the web interface.
2. Navigate to `System > Backup`.
3. Click on `Backup` to manually trigger a backup.

Remember, the backup files should be stored safely, preferably in a different location than your main system.

## Restore

1. Access the service's web interface.
2. Navigate to `System > Backup`.
3. Use the `Select Backup` option and upload your backup file.

For restoring, ensure that the service is stopped and then start it again after the restoration process. 
For Bazarr and Jackett, which do not have built-in backup and restore functionality, you'll need to manually copy the application directory for backup and replace it for restoration.

## Contributing

Pull requests and suggestions are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).
