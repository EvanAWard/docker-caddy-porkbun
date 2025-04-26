[![Docker](https://github.com/evanaward/docker-caddy-porkbun/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/evanaward/docker-caddy-porkbun/actions/workflows/docker-publish.yml) [![Check for Updates](https://github.com/evanaward/docker-caddy-porkbun/actions/workflows/check-update.yml/badge.svg)](https://github.com/evanaward/docker-caddy-porkbun/actions/workflows/check-update.yml)

# docker-caddy-porkbun

This is a custom [Caddy](https://hub.docker.com/_/caddy)-based image that adds the following features:

- adds the [porkbun](https://github.com/caddy-dns/porkbun) module to the base image
- installs the [`tzdata`](https://wiki.alpinelinux.org/wiki/Setting_the_timezone) package, so you can use the `TZ` environment variable

## Usage

The image is availabe on [GitHub Packages](https://github.com/evanaward/docker-caddy-porkbun/pkgs/container/docker-caddy-porkbun). You can use the `latest` tag or a specific Caddy version:

- `ghcr.io/evanaward/docker-caddy-porkbun:latest` (latest from GitHub)
- `ghcr.io/evanaward/docker-caddy-porkbun:2.9.1` (Caddy `2.9.1` from GitHub)

The following platforms are supported:

- `linux/amd64` (normal x64)
- `linux/arm64` (64-bit ARM, eg: Raspberry Pi 3/4)
- `linux/arm/v7` (32-bit ARM hard-float, eg: Raspberry Pi 2)

Don't forget to [update your config](https://github.com/caddy-dns/porkbun#config-examples) after pulling the image.

## License

See [LICENSE](./LICENSE) for more information.
