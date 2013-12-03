# goenv

Create a new go environment in the current working directory

This will create the dirs `bin`, `pkg` and `src`, update `$PATH` to include the newly created `bin` dir and update $GOPATH to be the current working directory.

# Installation

1. Download the script and put it on your $PATH (sometimes `/usr/local/bin`)

# Usage

## To create a new $GOPATH

1. mkdir new_gopath
2. cd new_gopath
3. . goenv

## To update $GOPATH

1. cd existing_gopath
2. . goenv
