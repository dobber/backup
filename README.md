# dobber/backup

## About
Generate a fast backup of a directory

I got sick of all the file-bak, dir-NEW, file-bogus files that were creeping my filesystems. After a few months I did not know where they came from and what was their contents. So I created a little bash script to date all those backup file.

## Install
After you clone the repo, just do `make` and it will copy the script to /usr/local/bin/backup

## Usage
Let's say you want to edit you httpd.conf, but before that, you need to create a backup version of the file.

	backup /etc/apache2/httpd.conf
	$EDITOR /etc/apache2/httpd.conf

That way, you have a backup copy named /etc/apache2/httpd.conf-201310301. The 201310301 translates to 2013-September-30 version 1. The version number is auto-increment.
