# Laboratory 09 — Cloud Automation Engineer

## Mission Overview

This activity focuses on using Bash scripts and Cron to automate a backup task. The goal is to create a backup of sample application data and schedule the script to run automatically.

## Objectives

- Understand basic Bash script syntax and variables.
- Create and execute a Bash script.
- Use `chmod` to change file permissions.
- Understand Cron scheduling.
- Document automation work using Markdown.

## Commands Executed

- `mkdir app-data` — creates the sample data folder.
- `echo "This is critical client data." > app-data/data.txt` — creates a sample data file.
- `nano backup.sh` — creates and edits the backup script.
- `chmod +x backup.sh` — makes the script executable.
- `./backup.sh` — runs the backup script.
- `ls -l backups/` — lists the generated backup files.
- `crontab -l` — displays the current Cron schedule.
- `env EDITOR=nano crontab -e` — opens the Cron editor.

## Skills Learned

I practiced writing a Bash script, creating a compressed backup, changing file permissions, and scheduling an automated task with Cron. I also practiced documenting commands and results in Markdown and managing files in GitHub.
