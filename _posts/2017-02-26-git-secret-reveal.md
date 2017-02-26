---
layout: post
title:  'git-secret-reveal'
date:   2017-02-26 18:27:18 +0300
permalink: git-secret-reveal
categories: command
---
git-secret-reveal - decrypts all added files.
=============================================

## SYNOPSIS

    git secret reveal [-f] [-d dir] [-p password]


## DESCRIPTION
`git-secret-reveal` - decrypts all the files in the `.gitsecret/paths/mapping.cfg` by running a `gpg --decrypt` command. It is important to have paired secret-key with one of the public-keys, which were used in the encryption.


## OPTIONS

    -f  - forces to overwrite exisiting files without prompt.
    -d  - specifies `--homedir` option for the `gpg`, basically use this option if your store your keys in a custom location.
    -p  - specifies password for noinput mode, adds `--passphrase` option for `gpg`.
    -h  - shows help.


## MANUAL

Run `man git-secret-reveal` to see this note.


## SEE ALSO

[git-secret-init(1)](http://git-secret.io/git-secret-init), [git-secret-tell(1)](http://git-secret.io/git-secret-tell), [git-secret-add(1)](http://git-secret.io/git-secret-add), [git-secret-hide(1)](http://git-secret.io/git-secret-hide)