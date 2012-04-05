
Bash utilities to work with github, matching my setup / workflow

## Description

Yet another uselessware.

I ♥ bash scripting, and I want to learn more.

I needed some kind of my very-own
mini[hub](https://github.com/defunkt/hub), eventually with git / bash as
the only required dependencies. That's it.


## Usage

    $ minihub
    Usage: minihub [command]

    Commands:

      browse              open the GitHub repository page
      clone               clone the git repo in $MINIHUB_PREFIX/<user>/<repo> location
      issue               open the given issue in default browser
      edit                Opens the project folder in the default editor
      help                print this msg

    Env:

      $MINIHUB_PREFIX    clone install location, defaults to ~/src.
      $MINIHUB_BROWSER   the browser that is called by minihub to open websites.
      $MINIHUB_EDITOR    the editor that is called by minihub with the edit
                         command, defaults to mvim.



    $ minihub clone mklabs minihub
    $MINIHUB_PREFIX unset, set to ~/src
    Cloned in /Users/mk/src/mklabs/minihub
    Initialized empty Git repository in /Users/mk/src/mklabs/minihub/.git/
    remote: Counting objects: 429, done.
    remote: Compressing objects: 100% (266/266), done.
    remote: Total 429 (delta 170), reused 381 (delta 122)
    Receiving objects: 100% (429/429), 125.79 KiB | 51 KiB/s, done.
    Resolving deltas: 100% (170/170), done.

    Cloned in /Users/mk/src/mklabs/minihub

    $ cd /Users/mk/src/mklabs/minihub

    $ minihub browse
    $MINIHUB_BROWSER unset, defaults to open.
    Opening https://github.com/mklabs/minihub in open browser

    $ minihub issue
    Opening https://github.com/mklabs/minihub/issues in open browser

    $ minihub issue 1
    Opening https://github.com/mklabs/minihub/issues/1 in open browser

    $ minihub edit mklabs minihub
    $MINIHUB_EDITOR unset, defaults to mvim.
    $MINIHUB_PREFIX unset, defaults to ~/src.
    Opening /Users/mk/src/mklabs/minihub in mvim editor


