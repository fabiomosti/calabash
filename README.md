# calabash
this is a simple Bash script collection to make some Debian administration task more easy :)

## installation
just clone or download the repository and merge the usr folder from the repository with the usr folder on your Linux box

### installation from web

    apt-get install wget && wget http://calabash.videoarts.it/va.current.tar
    tar -xvf ./va.current.tar --overwrite -C /

## config files
calabash uses a few config file to keep important informations at hand, these are usually located in /etc and
here are a short description for each one

### /etc/mysql.conf
if you install the MySQL/MariaDb server fron the `va.lamp.setup.sh` script, this file will be created with the
connection data needed for other `va.mysql.*` scripts to run; the file format is the one needed for use with the
`--defaults-file` parameter of most MySQL tools

## script

### wget script
these are script designed to make it easier to use wget in common tasks

#### va.wget.pages.list.sh
this script creates a simple list of all URLs from a web site; it is useful if you want a map of the site or so

usage:

`va.wget.pages.list.sh sourceSiteAddress listFileWithPath`

example:

`va.wget.pages.list.sh https://some.site.tld /tmp/urlsofsomesite.txt`