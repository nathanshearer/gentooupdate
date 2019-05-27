Description:
  Automatically update Gentoo Linux in phases:
    sync
    update
    preservedrebuild
    depclean
    revdeprebuild
    perlcleaner

Usage:
  gentooupdate [options]

Options:
  -a true
    Abort if there is unread news or if emerge is already running.
  -d, --depclean-args "--depclean"
    The arguments passed to emerge during the depclean phase.
  -e ""
    The arguments passed to revdep-rebuild during the revdeprebuild phase.
  -h, --help
    Display this help message and exit.
  -l, --perl-cleaner-args "--really-all"
    The arguments passed to perl-cleaner during the perlcleaner phase.
  -n, --nice N
    Sets the niceness to N (default 0).
  -r, --preserved-rebuild-args "@preserved-rebuild"
    The arguments passed to emerge during the preservedrebuild phase.
  -s, --sync-args "--sync"
    The arguments passed to emerge during the sync phase.
  -u, --update-args "-uDN --with-bdeps=y world"
    The arguments passed to emerge during the update phase.
  -v
    The same as --verbose 1.
  --verbose #
    Use more or less verbose output. Valid values are from 0 to 1 inclusive:
      0  Default. No output
      1  Show errors messages

Examples:
  gentooupdate -a false
  gentooupdate -n 20 -u "-uDN --with-bdeps=y --keep-going world"

Version:
  Gentoo Update 1.1.2.0
  Copyright (C) 2015 Nathan Shearer
  Licensed under GNU General Public License 2.0
