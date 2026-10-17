# Backup Script Guide

## 1. Purpose

The `backup.sh` script creates a compressed backup of the `app-data` folder. It uses a timestamp in the filename so each backup can have a different name.

## 2. Full Bash Script

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 3. Making the Script Executable

The command used is:

```bash
chmod +x backup.sh
```

The `chmod +x` command gives the file permission to run as a program. Without this permission, running `./backup.sh` may show a permission error.

## 4. Cron Job

The cron schedule used is:

```text
0 2 * * * /root/backup.sh
```

This schedules the script to run every day at 2:00 AM, assuming the script is located at `/root/backup.sh`.

### Cron Expression Breakdown

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

## 5. Expected Result

When the script runs successfully, it creates the `backups` folder if needed and saves a compressed `.tar.gz` file containing the `app-data` folder.
