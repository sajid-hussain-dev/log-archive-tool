# Log Archive Tool

A bash CLI tool that archives logs by compressing them into a tar.gz file.

## Usage
    sudo log-archive <log-directory>

## What it does
- Takes a log directory as an argument
- Compresses it into `logs_archive_YYYYMMDD_HHMMSS.tar.gz`
- Stores archives in `/var/log-archive` (override with `ARCHIVE_DIR`)
- Records the date and time of each archive in `archive.log`

## Install
    sudo cp log-archive /usr/local/bin/

## Schedule (daily at 2 AM)
    0 2 * * * /usr/local/bin/log-archive /var/log

## Skills practiced
Bash scripting, file and directory handling, tar, cron, CLI design
