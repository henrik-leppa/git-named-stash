Git Named Stash 1.1.0
=====================
[
  Encoding: UTF-8;
  Syntax: GitHub Flavored Markdown (GFM) <https://github.github.com/gfm/>;
]:#

POSIX/Unix shell command that allows using `git stash` command using the
stash's name/message.


[MIT License][]
---------------


[Changelog][]
-------------


Prerequisites
-------------

- POSIX/Unix shell
- `git` command


Usage
-----

```sh
git-named-stash show <name-of-stash> [<git-stash-arguments>...]
```
or:
```sh
git-named-stash drop <name-of-stash> [<git-stash-arguments>...]
```
or:
```sh
git-named-stash pop <name-of-stash> [<git-stash-arguments>...]
```
or:
```sh
git-named-stash apply <name-of-stash> [<git-stash-arguments>...]
```
or:
```sh
git-named-stash push <name-of-stash> [<git-stash-arguments>...]
```
or:
```sh
git-named-stash (--help | -H | -h | -?)
```
or:
```sh
git-named-stash (--version | -V | -v)
```

### Options

- `--help, -H, -h, -?`
  - Print the help message.
- `--version, -V, -v`
  - Print version and copyright information.

### Notes

- If there are multiple stashes with the same name/message, the one with the
  lowest index is used.

### Exit codes

- 0 (`EX_OK`): Successful exit
- 64 (`EX_USAGE`): Incorrect arguments supplied
- 69 (`EX_UNAVAILABLE`): Stash was not found

[(See `sysexits.h`)](https://www.freebsd.org/cgi/man.cgi?query=sysexits&sektion=3)


[Changelog]: ./CHANGELOG.md
[MIT License]: ./LICENSE.md
