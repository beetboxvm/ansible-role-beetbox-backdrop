# Ansible Role: Beetbox Backdrop

An Ansible role that creates and installs a Backdrop project on beetbox.

## Requirements

This role is specifically developed as an extension to beetbox -- https://github.com/drupalmel/beetbox

## Role Variables

Available variables are listed below, along with default values:

Checkout Backdrop project.
    
    backdrop_checkout: no
    
Backdrop project git respository. 
    
    backdrop_repo: "https://github.com/backdrop/backdrop.git"
    
Backdrop project version. This can be the full 40-character SHA-1 hash, the literal string HEAD, a branch name, or a tag name.
    
    backdrop_version: "HEAD"
    
Backdrop checkout depth. git is history truncated to the specified number or revisions
    
    backdrop_checkout_depth: 1
    
Install Backdrop project.
    
    backdrop_install_site: no
    
Backdrop install profile.
    
    backdrop_install_profile: standard
    
Backdrop admin account name.
    
    backdrop_account_name: admin
    
Backdrop admin account password.
    
    backdrop_account_pass: admin

## Dependencies

- Beetbox -- https://github.com/drupalmel/beetbox

## License

MIT