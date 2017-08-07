# Ansible Role: Beetbox Backdrop

[![Circle CI](https://circleci.com/gh/beetboxvm/ansible-role-beetbox-backdrop.svg?style=svg)](https://circleci.com/gh/beetboxvm/ansible-role-beetbox-backdrop)

An Ansible role that creates and installs a Backdrop project on beetbox.

## Role Variables

Available variables are listed below, along with default values:

Checkout Backdrop project.
    
    backdrop_checkout: no
    
Backdrop project git respository. 
    
    backdrop_repo: "https://github.com/backdrop/backdrop.git"
    
Backdrop project version. This can be the full 40-character SHA-1 hash, the literal string HEAD, a branch name, or a tag name.
    
    backdrop_version: "HEAD"
    
Backdrop checkout depth. git history truncated to the specified number or revisions.
    
    backdrop_checkout_depth: 1
    
Install Backdrop project.
    
    backdrop_install_site: no
    
Backdrop install profile.
    
    backdrop_install_profile: standard
    
Backdrop admin account name.
    
    backdrop_account_name: admin
    
Backdrop admin account password.
    
    backdrop_account_pass: admin


# beetbox

https://github.com/beetboxvm/beetbox

## Requirements

* [Composer](https://getcomposer.org/download/)
* [Vagrant](https://www.vagrantup.com/) >= 1.8
* [Virtualbox](https://www.virtualbox.org/)
* [Vagrant Hostsupdater](https://github.com/cogitatio/vagrant-hostsupdater)
* [Vagrant Auto-network](https://github.com/oscar-stack/vagrant-auto_network)

## Quickstart

  1. Open terminal (or [git bash](https://msysgit.github.io/) for windows users) and run the following commands --

  ```
  git clone https://github.com/beetboxvm/ansible-role-beetbox-backdrop.git backdrop && cd $_
  composer require --dev beet/box
  vagrant up
  ```

  2. Go to http://backdrop.local/

  ```
  username: admin
  password: admin
  ```

## License

MIT