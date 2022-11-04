# Installation

## General Steps

These are the steps required to install Leantime. They work for most configurations.

* Download latest release package
* Create an empty MySQL database
* Upload entire directory to your server 
* Point your domain to the `public/` directory
* Rename `config/configuration.sample.php` to `config/configuration.php`
* Fill in your database credentials (username, password, host, dbname) in `config/configuration.php`
* Navigate to `<yourdomain.com>/install`
* Follow instructions to install database and set up first user account

Updates

As of v2.2.8 all Leantime packages contain an update script called "updateLeantime.sh". Place this file into your current installation folder. See below example:

user@leantime-server:/var/www/html/leantime$ sudo ./updateLeantime.sh


The below script with will run and detect the new release. A backup is recommended in case a recovery is needed. 


    _                 _   _
   | |   ___ __ _ _ _| |_(_)_ __  ___
   | |__/ -_) _` | ' \  _| | '  \/ -_)
   |____\___\__,_|_||_\__|_|_|_|_\___|      _
                     | | | |_ __  __| |__ _| |_ ___ _ _
                     | |_| | '_ \/ _` / _` |  _/ -_) '_|
                      \___/| .__/\__,_\__,_|\__\___|_|
                           |_|


For correct operation of this script, please ensure you have zip, unzip, wget and curl installed.

There is an update available!
Do you want to update from v2.2.7 to v2.2.10? [Y/n] y
Do you want to create a backup before updating (recommended) [Y/n]y

Creating a backup in the 'backup' folder
 - retrieving the database connection details (Done)
 - Backing up the database in backup/leantime_db_backup_20221104_102355.sql.gz WARNING: Forcing protocol to  TCP  due to option specification. Please explicitly state intended protocol.
(Done)

 - Backing up the files in backup/leantime_file_backup_20221104_102355.zip
(Done)


Starting the update process
 - Downloading the updatefile (Leantime-v2.2.10.zip) in the 'update' folder (Done)

 - Extracting the updatefile (Done)

 - Applying the update (Done)

 - Cleaning up the temporary files (Done)

Leantime has been succesfully updated
