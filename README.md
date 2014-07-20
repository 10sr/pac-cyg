pac-cyg
=======

A command-line installer for Cygwin which cooperates with Cygwin Setup and uses
the same repository. The syntax is similar to `pacman` from Arch Linux.


Basic Usage
-----------

To install packages, issue `pac-cyg -S tmux`.
Type `pac-cyg -Qs` to search installed packages, and `pac-cyg -R tmux`
to remove.


Synopsis
--------

    pac-cyg <operation> [<option> ...] [<target> ...]

    Operations:
        -S    Sync packages
        -Q    Query installed packages
        -R    Remove packages
        -V    Show version

    use 'pac-cyg -h' with an operation for available options


### -S ###

Synchronize packages (installing, searching remote repositories, ...).
Available options are:

    -s <query>   Search repositories
    -i <package> Show infos about packages
    -y           Update repository databases
    -h           Print this help

No option to install packages.


### -Q ###

Query to view installed packages. Available options are:

    -s <query>   Search installed packages
    -i <package> Show infos about installed packages (very simple)
    -o <file>    Find package that has given files or commands
    -l <package> List files owned by packages
    -h           Print this help


### -R ###

Remove installed packages.


License
-------

This software is released under the GNU General Public License. See LICENSE for
details.


Acknowledgment
--------------

`pac-cyg` is a fork project of [apt-cyg](https://code.google.com/p/apt-cyg/) by
Stephen Jungels, which provides an apt-get like interface for managing packages.
Thanks!
