pac-cyg
=======

A command-line installer for Cygwin which cooperates with Cygwin Setup and uses
the same repository. The options are similar to `pacman` of Arch Linux.


Basic Usage Examples
-----------

To install packages, issue `pac-cyg -S tmux`.
Type `pac-cyg -Qs` to search installed packages, and `pac-cyg -R tmux`
to remove.

You have to run `pac-cyg -Sy` at least once to search or install packages.


Options
--------

    pac-cyg <operation> [<option> ...] [<target> ...]

    Operations:
        -S    Sync packages
        -Q    Query installed packages
        -R    Remove packages
        -V    Show version

Use 'pac-cyg -h' with an operation for available options for that operation.


### -S (Sync) ###

Synchronize packages (installing, searching remote repositories, ...).
Available options are:

    -s <query>   Search repositories
    -i <package> Show infos about packages
    -y           Update repository databases
    -h           Print this help

No option to install packages.


### -Q (Query) ###

Query to view installed packages. Available options are:

    -s <query>   Search installed packages
    -i <package> Show infos about installed packages (very simple, use -Si for
                 details)
    -o <file>    Find package who owns given files or commands
    -l <package> List files owned by packages
    -h           Print this help


### -R (Remove) ###

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
