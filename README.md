# Provisioning for my macbook

## How to setup

```bash
## command line tools
xcode-select --install

## install homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

## install ansible
brew install ansible

## install zsh
brew install zsh
sudo echo /usr/local/bin/zsh >> /etc/shells
chsh -s /usr/local/bin/zsh

## install git
brew install git

## clone this repository
git clone https://extra-ghe.dev.gree-dev.net/kazuki-k-ito/provisioning.git
```

## Execute

Run all roles

```bash
ansible-playbook playbook.yaml
```

Run specific role with tags

```bash
ansible-playbook playbook.yaml -t homebrew
```
