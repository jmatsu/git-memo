# Enhanced Git notes

## What's Git notes?

Git notes can add annotations to commits w/o changing their hash.

Show [Git SCM](http://git-scm.com/docs/git-notes)

## Installation

Download `git-memo`, apply executable permission to it and put it in your `$PATH`

or add `bin` to your `$PATH`

## Motivation

As you know, `git-notes` would conflict with same namespace notes.

Default, `git-note` uses `commits` as it. You must input `--ref $namespace` if you would like to change namespace.

In addition, `git-notes` will not be published/retrieved until running explicit command excecution.
e.g. `git push $remote refs/notes/*`, `git fetch $remote refs/notes/*:refs/notes/*`

## How to use

This can also work as `git-notes`, so you can use this instead of `git-notes`.

### Create refs name and use it

At first time to execute `git-memo`, `git-memo` requires your author name and saves it to `memo.user.name` in config.

`git-memo` always use `memo.user.name` if `--ref` is not specified.

### push and fetch

If you would like to publish your notes, run `git memo push $remote`.

If you would like to retrieve all notes, run `git memo fetch $remote`.
