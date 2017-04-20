# twython-sysinfo
Twython script containing system information with optional attachment of snapshots created by motion.

The string `# coding: utf-8` is necessary for correct formatting of umlauts.

Based on djfav's gists over at https://gist.github.com/djfav

## Available stats
### Date and time
* `time`
### CPU temperature
* `temp`
### Memory usage
* `tr(usedmb)`
* `str(totalmb)`
* `str(percent)`
### Network
*`ip` (language specific) 
** available: en, de
** standard: de
## Installation
* Install twython
* Optional: Install motion and configure snapshots to be taken 
* Clone this repo
* Change `your_data` to the strings from you own twitter app
* Optional: Uncomment one of the lines starting wit `api.` depending on the usage of snapshots