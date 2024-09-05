# shailesh-aws-labs

# LAMP Stack Setup Script

This repository contains a shell script for setting up a LAMP (Linux, Apache, MySQL, PHP) stack on an Amazon Linux system. The script automates the installation and configuration of necessary components for running a web application.

## Features

- Installs and configures Apache web server
- Sets up PHP and required extensions
- Installs MariaDB (MySQL-compatible database)
- Downloads and extracts a sample PHP application
- Installs the AWS SDK for PHP

## Prerequisites

- Amazon Linux 2 or compatible system
- Root or sudo access

## Usage

1. Clone this repository or download the script.
2. Make the script executable:
   ```
   chmod +x setup_lamp.sh
   ```
3. Run the script with root privileges:
   ```
   sudo ./setup_lamp.sh
   ```

## What the Script Does

1. Installs the LAMP stack components:
   - Apache web server (httpd)
   - PHP and necessary extensions
   - MariaDB server

2. Starts and enables the Apache web server

3. Downloads and extracts a sample PHP application to `/var/www/html/`

4. Installs the AWS SDK for PHP in `/var/www/html/vendor/`

5. Updates existing packages

## Notes

- The script assumes you're running it on an Amazon Linux 2 system or a compatible distribution that uses `dnf` as the package manager.
- Make sure you have an active internet connection when running the script, as it needs to download packages and files.
- After running the script, you may need to configure your database and adjust PHP settings according to your specific requirements.

## Security Considerations

- This script is intended for development or testing environments. For production use, additional security measures should be implemented.
- It's recommended to change default passwords, configure firewalls, and follow best practices for securing your LAMP stack.

## Contributing

Feel free to fork this repository and submit pull requests for any improvements or fixes.

