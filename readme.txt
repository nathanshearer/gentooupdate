Synopsis
  Automatically update Gentoo Linux in phases:
    sync
    update
    preservedrebuild
    depclean
    revdep

Usage:
  gentooupdate [options]

Options:
  -a true
    Abort if there is unread news or if emerge is already running.
  -d "--depclean"
    The arguments passed to emerge during the depclean phase.
  -e ""
    The arguments passed to revdep-rebuild during the revdeprebuild phase.
  -h
    Display this help message and exit.
  -n N
    Sets the niceness to N (default 0).
  -r "@preserved-rebuild"
    The arguments passed to emerge during the preservedrebuild phase.
  -s "--sync"
    The arguments passed to emerge during the sync phase.
  -u "-uDN --with-bdeps=y world"
    The arguments passed to emerge during the update phase.

Examples:
  gentooupdate -a false
  gentooupdate -n 20 -u "-uDN --with-bdeps=y --keep-going world"

Version:
  Gentoo Update 1.1.0.0
  Copyright (C) 2015 Nathan Shearer
  Licensed under GNU General Public License 2.0
