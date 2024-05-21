# Automated Backup System

## Overview
This project provides an automated backup solution for critical directories using a shell script. It ensures data integrity and availability by creating daily backups and rotating them based on your specified retention policy.

## Features
- **Automated Backups**: The shell script automatically backs up specified directories to an external drive.
- **Retention Policy**: Backups are categorized as daily, weekly, and monthly, with a specified retention count for each category.
- **Cron Job**: Scheduled tasks ensure backups run without manual intervention.
- **Notifications**: Successful backups trigger a cURL request to a specified endpoint (Webhook).

## Prerequisites
- Linux-based system (tested on Ubuntu)
- [rclone](https://rclone.org/) installed (for cloud storage integration)

## Installation
1. Clone this repository:
   ```
   git clone https://github.com/PurushotamSharma/Automated-Backup-and-Rotation-Script.git
   ```

2. Configure the script:
   - Edit `backup_script.sh` and set the required variables (explained in the script comments).

3. Install rclone:
   ```
   sudo apt-get install rclone
   ```

4. Configure rclone:
   - Run `rclone config` to set up a new server (e.g., Google Drive).

5. Schedule backups:
   - Set up a Cron job to run the script at desired intervals.

6. Test:
   - Run the script manually to verify backups.

## Usage
- Customize the script according to your project's needs.
- Update the README with detailed instructions for other users.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to add more sections or elaborate on specific aspects of your project. Once you've created the README, commit it to your GitHub repository. Happy coding! 🚀.

If you need further assistance or have any questions, feel free to ask! 😊
