# wpspeed
A few WordPress a server performance tests

## How to use this tool
Once you have made a SSH connection to an account with wordpress installed run this command:

    . <(curl -sS https://raw.githubusercontent.com/miles-cm/wpspeed/master/wpspeed)

## Available commands:
**wpspeed**
* Checks if gzip compression exists in the .htaccess file.
* Checks if database cleanup plugins are installed (such as wp-speed or wp-optimize).
* Checks if image compression plugins are installed (such as tiny-compress-images or ewww-image-optimizer).
* Checks if caching plugins are installed (such as w3-total-cache or wp-super-cache).
* Checks if browser cache rules are present in the .htaccess file.
* Lists the number of plugins and suggests the use of p3-profiler (a plugin that helps pinpoint plugin lag) if not installed.

**wpspeed -p, --plugins**
* Show how many times the site calls to each plugin per page load

**wpspeed -h, --help**
* Displays a list of available commands

**loadhistory**
* See when the load on the server was high in the last 30 days using sar logs.

**apps**
* List of installed applications and their paths. (This command is just an alias for "cat ~/tmp/installedapps.yml" )
