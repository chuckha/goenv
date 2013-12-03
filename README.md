# goenv

Create a new go environment in the current working directory

This will create the dirs `bin`, `pkg` and `src`, update `$PATH` to include the newly created `bin` dir and update $GOPATH to be the current working directory.

# Installation

1. Download the script and put it on your $PATH (sometimes `/usr/local/bin`)

# Usage

## To start a new Go project

2. mkdir new_project
3. cd new_project
4. . goenv

## To change environments to an existing Go project

1. cd existing_proj
2. . goenv
