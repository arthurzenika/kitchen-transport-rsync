# kitchen-transport-rsync

[![Build Status](https://api.travis-ci.org/unibet/kitchen-transport-rsync.svg)](https://travis-ci.org/skillfox/kitchen-transport-rsync)


This transport is based on rsync over ssh providing dramatic performance improvements.
It will only work with if rsync is be available in the PATH on both local and remote end points.

This is a fork of https://github.com/kindredgroup/kitchen-transport-rsync the original library is published on rubygems : [![Gem Version](https://badge.fury.io/rb/kitchen-transport-rsync.svg)](http://badge.fury.io/rb/kitchen-transport-rsync)

Only passwordless (using ssh key pair) communication is supported at the moment.

## Recommended **.kitchen.yml** snippet to activate Rsync transport

```
transport:
  name: rsync
  ssh_key: ~/.vagrant.d/insecure_private_key
  username: vagrant
```

## Gemfile
```
gem 'kitchen-transport-rsync'
```
