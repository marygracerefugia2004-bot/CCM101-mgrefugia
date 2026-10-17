# Laboratory 09 — Cloud Automation Engineer

## Mission Overview

Congratulations! Your ability to secure cloud environments has proven that you are ready for the highest level of operations. You have been promoted to the Cloud Automation and DevOps Team at CloudNova Technologies.

Until now, you have been working as a traditional systems administrator, typing commands manually one by one. In large enterprise environments with thousands of servers, manual administration is too slow and can easily lead to human errors. To manage these systems efficiently, you need to learn automation.

Using the KillerCoda Playground, you will take on the role of a Cloud Automation Engineer. You will learn the basics of Bash shell scripting, create an automated backup routine, assign executable permissions, and configure the Linux Cron scheduler to run your script automatically.

**Remember:** If you have to do a task more than twice in the cloud, you should automate it.

## Objectives

At the end of this laboratory activity, you should be able to:

- Understand the basic syntax of a Bash shell script, including variables and basic commands.
- Use the command-line text editor `nano` to write and save executable scripts.
- Modify Linux file permissions using the `chmod` command.
- Understand task scheduling and the syntax of a Linux crontab.
- Document automation code and Cron job configurations using Markdown.
- Complete the final chapter of your GitHub Cloud Computing Portfolio.

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
