# linux-backup
backup script for Linux machines

## Installation

Go to the directory where you want to store the files

```
cd <your desired folder>
```

Clone this repo

``` bash
git clone https://<this repo>
```


## Code

Options:

1. Create Backup
2. Sync Backup (to some external device / folder)
3. Enter settings

In the beginning: "Initialise" -> Creates "settings"-folder, and the user is required to enter custom settings or confirm default values.

Important:

* The script creates a "settings"-folder which should be ignored by git, in case there are modifications to the source code
* The script stores the backups by default in the `<repo>/backups` folder, it should be added to gitignore too, maybe that can be changed in settings in the future

### Folder

```
├── README.md
├── script.sh
├── .git
├── .gitignore
├── settings
│   ├── settings.json / settings.cfg
├── backups
│   ├── backup_01-01-1970.tar

```

### Settings

* excluded directories
* included directories (if child of an excluded dir)
* 


#### Defaults

> OS specific variations should be included in the future – at the moment, this script is for Debian-based systems only


### Requirements

* git
* tar
