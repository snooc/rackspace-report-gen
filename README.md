# RACKSPACE REPORT GENERATOR

One day I found out that our Cloud Sites account for ForeFront was nearing its disk usage quota. I knew that there were no way that we actually were using 90GB. So I went on a search to figure out what websites were using the most data. During my research, I found out that Rackspace does not allow you to view disk usage on a site level, so I hit up my boy Ed at Rackspace Fanatical Support and he hooked me up with a generic text file report of all of the folders in our account.

This was awesome, but I was too lazy to go through 1800 lines of data, plus file sizes were not using consistent units. 

This is what I wrote this! It take in the input, parses each line, converts everything to kilobytes, sorts by smallest to biggest, then prints everything out. I was able to use this and find a couple rogue backups from 2012 that were going daily for the past two years.

This saved me a lot of time and could be used to find many other things...like how many backup directors you have, etc.

## Installation

    $ bundle install

## Using
To use just:

     $ rackspace-report-gen foo.txt

#### Extra notes
I threw in a Gemfile to be nice.