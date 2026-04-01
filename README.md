# jellyfin-stack

This repository contains the configuration for my Jellyfin deployment.

## Environment Setup
The stack relies on the following environment variables:

| Variable | Description | Example |
| :--- | :--- | :--- |
| `URL` | Jellyfin server URL | `https://jellyfin.domain.tld` |

## Persistent Storage
I use bind mounts for data persistence. Ensure these paths exist on the Docker host:
* `/opt/docker/jellyfin/config` - Config files for Jellyfin
* `/opt/docker/jellyfin/cache` - Jellyfin cache
* `/opt/docker/jellyfin/series` - Storage for series
* `/opt/docker/jellyfin/movies` - Storage for movies

---

[Back to Homelab Overview](https://github.com/KubaMichalowski-homelab)
