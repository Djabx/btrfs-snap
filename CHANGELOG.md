# btrfs-snap Changelog

## v1.3.X-develop (Aug 27 2015)
* Added checks for existing snapshots and use pattern to search for existing snapshots

## v1.3.2 (Jan 10 2015)
* added switch to generate more compatible snapshot names
  (no colons in file names: this confuses SAMBA/Windows clients)

## v1.3.1 (Jan 05 2015)

* added switch to override default snapshot directory name ".snapshot"
* cleanup

## v1.2.2 (Sept 24 2013)

* trailing slash removal failed on multipart paths due to missing line
  terminator.  Time for a bats test suite.

## v1.2.1 (Sept 24 2013)

* fix trailing slash removal so that it works when the mountpoint is '/'.
  This required a change to perl from sed (standard sed doesn't have negated
  character classes)

## v1.2.0 (Sept 21 2013)

* added VFS snapshot naming support courtesy of gitmopp

## v1.1.0 (July 30 2013)

* add README
* add readonly snapshot and base directory features

## v1.0.0 (July 20 2013)

* Initial version written by Birger Monsen <birger@birger.sh>
