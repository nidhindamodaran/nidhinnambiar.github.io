---
layout: post
---

Ruby Version Manager(**RVM**), is for managing multiple installations of Ruby on same machine.The different versions can then be switched between to enable a developer to work on several projects with different version requirements

####1.Download script

```bash
\curl -sSL https://get.rvm.io | bash -s stable
```
This will install latest release version,

For latest development state

```bash
\curl -sSL https://get.rvm.io | bash
```
####2.Load RVM into your shell as a function

```bash
source /etc/profile
```
####3.Reload shell configuration & test

```bash
source ~/.rvm/scripts/rvm
```
Type below in terminal and will show RVM is a function
```bash
type rvm | head -n 1
rvm is a function
```
####4.Installing specific versions of ruby using rvm
```bash
rvm list known
```
This will list all ruby binaries known.

For installing a specific version in list (eg. 2.2.2)
```bash
rvm install 2.2.2
```
After installing, we can choose ruby version as
```bash
rvm use 2.2.2
```
Also we can set default ruby versons
```bash
rvm use 2.2.2 --default
```

Enjoy using RVM
