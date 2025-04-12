🛡️ Automated Backup Script – backup.sh

A simple, reliable bash script to automatically archive and back up files that have been modified in the last 24 hours. Built as part of the “Hands-on Introduction to Linux Commands and Shell Scripting” course by IBM on Coursera.
📁 Project Overview

Imagine you’re working at a company that stores encrypted password files. Interns used to manually back them up every day — a process prone to human error and inefficiency. This project automates that daily backup task using basic Linux commands and shell scripting.
📜 Features

    ✅ Accepts source and destination directories as arguments

    📦 Archives files modified within the last 24 hours using tar

    🔐 Ideal for backing up sensitive or encrypted data

    🕒 Can be scheduled with cron for full automation

🔧 How It Works

    Takes two arguments:

        Target directory (source of files)

        Destination directory (where backup will be saved)

    Identifies all files updated in the last 24 hours

    Archives them into a timestamped .tar.gz file

    Moves the archive to the destination directory

🧪 Example Usage

./backup.sh important-documents /home/user/backups

📅 Automation with Cron

To schedule the script to run every day at midnight:

0 0 * * * /usr/local/bin/backup.sh /home/user/important-documents /home/user/backups

Make sure the script is executable:

chmod +x backup.sh

And copy it to a system path if needed:

sudo cp backup.sh /usr/local/bin/

🗂️ File Structure

.
├── backup.sh
├── README.md
└── (Optional) screenshots/         # For submission or visual output

🎓 Built With

    Bash scripting

    Core Linux utilities (tar, date, chmod, touch)

    Cron jobs for scheduling

🏅 Certificate

This project is part of the IBM course “Hands-on Introduction to Linux Commands and Shell Scripting.”
📜 View Certificate: Coursera Verified Certificate
🙋‍♂️ Author

Awab Milan
📌 Electrical & Embedded Systems Enthusiast
📬 GitHub Profile
