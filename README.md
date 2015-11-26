# Spider Vagrant

[![Build status](https://travis-ci.org/JFK/spider-vagrant.svg?branch=master)](https://travis-ci.org/JFK/spider-vagrant)

## Preparation

* Vagrant
* ansible

## What gets installed:

* Python2.7, Pip & VirtualEnv
* ntp
* mongodb
* redis
* Nignx
* rq

## Let's get rolling!

Before run ```vagrant up```, you may need to do...

```
$ ssh-add  ~/.ssh/id_rsa
$ echo 'ForwardAgent yes' >> ~/.ssh/config
```

Setup

```
$ git clone git@github.com:JFK/spider-vagrant.git
$ cd spider-vagrant
$ vagrant up
```

In order to access the site, configure hosts file.

```
$ echo "192.168.33.11 <server_name>" | sudo tee -a /etc/hosts
```

## Contribute

If you have any suggestions, feel free to create an issue here on Github and/or fork this repo, make changes and submit a pull request!
