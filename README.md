<p align="center">
  <img src="icon.png" alt="Scryer" width="180" />
</p>

# Scryer for Unraid

Official Unraid Community Apps template for
[Scryer](https://github.com/scryer-media/scryer), a self-hosted, all-in-one
media automation platform for movies, TV series, and anime. Scryer combines
library management, discovery, requests, acquisition, imports, and subtitles
in one efficient application with an embedded web interface.

## What Scryer Replaces

Scryer can replace several separate applications with one coordinated system:

- **Radarr** for movie monitoring, searching, upgrades, importing, renaming,
  and organization
- **Sonarr** for TV series and anime monitoring, episode tracking, searching,
  upgrades, importing, renaming, and organization
- **Seerr** for discovery, user requests, request queues, and approval workflows
- **Bazarr** for subtitle discovery, acquisition, and management

Scryer was written from scratch and is not affiliated with the Servarr
projects.

## Major Features

- Unified movie, TV series, and anime catalogs with monitoring, wanted,
  calendar, history, and activity views
- Discovery recommendations plus multi-user request and approval workflows
- Pluggable indexers, download clients, subtitle providers, notifications, and
  media-server integrations
- Quality and delay profiles, custom release rules, cutoff upgrades, and
  automated release selection
- Coordinated downloads, imports, file renaming and organization,
  post-processing scripts, and recycle-bin recovery
- Automated subtitle searching and management
- Multilingual metadata and an interface that follows the selected language
- User access controls, authentication, API keys, security and audit tooling,
  encrypted credentials, and backup/restore
- Responsive embedded web UI, GraphQL API, scheduled jobs, logs, and health
  monitoring in an efficient compiled Rust service

## Container

- Image: `ghcr.io/scryer-media/scryer:latest`
- Web UI: container port `8080`
- Persistent configuration: `/config`
- Optional libraries: `/data/movies`, `/data/series`, and `/data/anime`

The media-library mappings are optional. They can be added during installation
or later when Scryer is ready to manage files on the Unraid host.

Scryer creates `/config/encryption.key` with mode `0600` when no external key
is supplied. Preserve `/config`; it contains Scryer's database, settings,
metadata, and the key required to decrypt stored credentials.

## Screenshots

### Overview

![Scryer overview](https://raw.githubusercontent.com/scryer-media/scryer-unraid/main/screenshots/01-overview.webp)

### Anime Library

![Scryer anime library](https://raw.githubusercontent.com/scryer-media/scryer-unraid/main/screenshots/02-anime-library.webp)

### Discovery

![Scryer discovery](https://raw.githubusercontent.com/scryer-media/scryer-unraid/main/screenshots/03-discovery.webp)

### Request

![Scryer request queue](https://raw.githubusercontent.com/scryer-media/scryer-unraid/main/screenshots/04-request.webp)

### Import

![Scryer import setup](https://raw.githubusercontent.com/scryer-media/scryer-unraid/main/screenshots/05-import.webp)

## Support

- [Getting started](https://www.scryer.media/scryer/docs/getting-started/)
- [Issue tracker](https://github.com/scryer-media/scryer/issues)
- [Discord](https://discord.gg/SQmtZTanqm)
- [Reddit](https://www.reddit.com/r/scryer_media/)
- [Source code](https://github.com/scryer-media/scryer)

## Licensing

The files in this template repository are licensed under the MIT License.
Scryer itself is licensed under the
[GNU General Public License version 3](https://github.com/scryer-media/scryer/blob/main/LICENSE).
