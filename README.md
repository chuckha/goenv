# goenv

Create a new Go workspace in the current working directory and
launch a subshell with the correct `$GOPATH` and `$PATH` variables.

Note for OS X users and possibly others: subshells will source your .bashrc
but not your .bash_profile.

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

## To create a new Go workspace

1. `$ mkdir new_goworkspace`
2. `$ cd new_goworkspace`
3. `$ goenv`

## To use an existing Go workspace

1. `$ cd existing_goworkspace`
2. `$ goenv`
