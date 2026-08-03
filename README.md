<p align="center">
  <img src="icon.png" alt="Scryer" width="180" />
</p>

# Scryer for Unraid

Official Unraid Community Apps template for
[Scryer](https://github.com/scryer-media/scryer), a self-hosted media
management application for movies, TV series, and anime.

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
