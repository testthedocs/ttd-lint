# ttd-lint

ttd-lint is a linter for checking certain words.

[![asciicast](https://asciinema.org/a/b8s34cplg3aqnztly3pe3pt03.png)](https://asciinema.org/a/b8s34cplg3aqnztly3pe3pt03)

## Install

```bash
npm install ttd-lint -g
```

## Usage

This will check all files in the `docs` directory

```bash
ttd-lint docs
# Github
docs/index.rst:5:Github

Found certain words, please resolve it.
```

## Configure

~/.ttd-lintrc or ./.ttd-lintrc

```txt
Github
Javascript

describe\.only(
it\.only(
```

### Difference of this fork

- ttd-linter is checking case sensitive and for the exact match
- ttd-linter is tested against [shellcheck](https://www.shellcheck.net/)

**Please note**, `ttd-lint` is only tested on Ubuntu 16.10 and Debian 8.
