# goenv

Create a new Go environment in the current working directory.

This will create the dirs `bin`, `pkg` and `src`, update
`$PATH` to include the newly created `bin` dir and update
`$GOPATH` to be the current working directory.

# Why?

Using per-project dependencies removes the possibility of version conflicts
between projects. If Project A requires package Xv1.0 and Project B requires
package Xv2.0, but the required packages share an import name
("github.com/user/package"), it's impossible to have both dependencies
installed in the same Go workspace without a headache.

One solution is to have a copy of each projects dependencies isolated from
each other by modifying `$PATH` and `$GOPATH` if you switch projects.

This script makes that process of changing environment variables easier.

# Installation

1. Download the script and put it on your $PATH (sometimes `/usr/local/bin`)

# Usage

## To create a new $GOPATH

1. `$ mkdir new_gopath`
2. `$ cd new_gopath`
3. `$ . goenv`

## To update $GOPATH

1. `$ cd existing_gopath`
2. `$ . goenv`
