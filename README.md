# Docker Container for WHMCS

A WHMCS 8.1.3 developer environment for Docker forked from [darthsoup](https://github.com/darthsoup/docker-whmcs).

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)

## Installation

1. Clone this repository and copy the WHMCS installation archive to the `./whmcs` directory.
2. Copy `.env.example` to `.env`, fix `WHMCS_PATH_URL` and `WHMCS_PATH_DOCKER`.
3. Insert `dump.sql` to `/mysql/docker-entrypoint-initdb.d` folder.
4. Update `/whmcs/configuration.php` file.

### Requirements

1. Database backup `dump.sql`.
2. WHMCS configuration file.

### Tested WHMCS Versions

* [X] 8.1.3

## Usage

Start the container with:

```bash
docker-compose up
```

The WHMCS database import itself takes 2-3 minutes.

## Authors

- [@darthsoup](https://github.com/darthsoup)
- [@laradock](https://github.com/laradock/laradock)
