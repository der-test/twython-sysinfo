# twython-sysinfo
Twython script containing system information with optional attachment of snapshots created by motion.

The string `# coding: utf-8` is necessary for correct formatting of umlauts.

## Installation
* Install twython
  * `sudo apt install twython`
* Optional: Install dnsutils to display external IP (dig)
  * `sudo apt install dnsutils`
* Optional: Install motion
  * `sudo apt install motion`
  * Configure snapshots to be taken (config details will be added later)
  * Add `input -1` to the end of /etc/motion/motion.conf to avoid problems with USB cameras
* Clone this repo
  * `git clone https://github.com/der-test/twython_sysinfo`
* Open downloaded folder
    * `cd twython-sysinfo`

## Configuration
* Edit the configuration
  * `nano config.ini`
  * Change `your_data` to the strings from you own twitter app
* `tweet` may contain escaped text like `Some text:` and the available stats like `time+`(first element in the tweet, `+time+`(between) and `+time` (last element).
* twysinfo_media.py
  * `photo` path needs to be changed if not using motion standard config

### Available stats
#### Date and time
* `time`
#### CPU temperature
* `temp`
#### Memory usage
* `str(usedmb)`
* `str(totalmb)`
* `str(percent)`
#### Network
* `ip` (language specific)
  * available: en, de
  * standard: de
* `extip`

Based on djfav's gists over at https://gist.github.com/djfav
