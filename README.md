# Ansible playbook for Mac setup

This is playbook to install and configure software on a Macbook used for cloud native development.

It is continually evolving and leans heavily on the following examples on Github:

* [geerlingguy/mac-dev-playbook](https://github.com/geerlingguy/mac-dev-playbook)
* [BattleSchool](http://spencer.gibb.us/blog/2014/02/03/introducing-battleschool)
* [osxc](https://github.com/osxc)
* [MWGriffin/ansible-playbooks](https://github.com/MWGriffin/ansible-playbooks)

## Installation

Run the installer script...

```shell
curl -fsSL https://raw.githubusercontent.com/bmacauley/ansible-playbook-mac-dev/master/install | bash
```

The installer script installs Apple's command line tools, Homebrew, Python Pip, Ansible and finally it downloads and runs this playbook

## Defaults

Not everyone's development environment and preferred software configuration is the same.

You can override any of the defaults configured in default.config.yml by creating a config.yml file and setting the overrides in that file. For example, you can customize the installed packages and apps with something like:

## Ansible roles used
- [geerlingguy.homebrew](https://github.com/geerlingguy/ansible-role-homebrew)
- [ansible-role-dotfiles](https://github.com/bmacauley/ansible-role-dotfiles)
- [ansible-role-sublimetext](https://github.com/bmacauley/ansible-role-sublimetext)
- [ansible-role-mas]( https://github.com/bmacauley/ansible-role-mas)


## Other repos used
- [dotfiles](https://github.com/bmacauley/dotfiles.git)
- [zsh-git-prompt](https://github.com/bmacauley/zsh-git-prompt.git)
- [poerline fonts](https://github.com/powerline/fonts.git)
- [Vundle(vim)](https://github.com/gmarik/Vundle.vim.git)


## Included Applications

Applications (Homebrew Casks):

  ### Cloud Tools ##
  - awscli
  - aws-sam-cli
  - aws-shell
  - consul
  - docker
  - docker-clean
  - docker-compose
  - heroku
  - heroku-toolbelt
  - minikube
  - nomad
  - packer
  - packer-completion
  - s3cmd
  - terragrunt
  - terraform-docs
  - tfenv
  - vagrant
  - vagrant-completion
  - vault
  ### Git Tools ##
  - act
  - gist
  - git
  - git-crypt
  - hub
  - tig
  ### Unix Tools ##
  - bash
  - bash-completion
  - battery
  - brew-cask-completion
  - bundler-completion
  - cloc
  - curl
  - direnv
  - htop-osx
  - gpg
  - gpg2
  - libevent
  - libffi
  - libvterm
  - libxml2
  - libyaml
  - jq
  - nmap
  - openssl
  - tmux
  - tree
  - wget
  - wrk
  ### MacOS Tools ##
  - launchctl-completion
  - mas
  - openvpn
  - zsh-completions
  - zenith

  ### Development Tools ##
  - brave-browser
  - docker
  - discord
  - firefox
  - github
  - google-chrome
  - gpg-suite
  - keybase
  - microsoft-teams
  - postman
  - virtualbox
  - visual-studio-code
  - zoom

  ### Mac AppStore Tools ##
  - 497799835   # Xcode
  - 408981434   # iMovie
  - 409183694   # keynote
  - 1116599239  # NordVPN IKE - Unlimited VPN
  - 1475387142  # Tailscale
  - 1333542190  # 1Password
  - 972572731   # MoneyPro
  - 431748264   # PluralSight
  - 803453959   # Slack
  - 1147396723  # Whatsapp Desktop
  - 1153157709  # SpeedTest
  - 1559269364  # Notion
  - 409201541   # Pages
  - 462054704   # Word
  - 462058435   # Excel
  - 462062816   # Powerpoint
  - 409203825   # Numbers

## Testing the Playbook
Instructions to build a Mac OS X VirtualBox VM(geerlingguy), on which you can continually run and re-run this playbook to test changes and make sure things work correctly.