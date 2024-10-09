# formation-gitlab

## Installation
- Suivre le lien suivant pour l'installation : https://about.gitlab.com/install/#ubuntu


### 1. Install and configure the necessary dependencies
```
sudo apt-get update
sudo apt-get install -y curl openssh-server ca-certificates tzdata perl
```
### install Postfix
```
sudo apt-get install -y postfix
```
### Add the GitLab package repository and install the package
```
curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh | sudo bash
```
### Next, install the GitLab package
```
sudo EXTERNAL_URL="http://gitlab.example.com" apt-get install gitlab-ee
```
### Add gitlab.example.com to your /etc/hosts next to 127.0.0.1
```
connect from your browser to http://gitlab.example.com
```
### Browse to the hostname and login
```/etc/gitlab/initial_root_password```. Use this password with username root to login.

## Notes
password reset to root / aymenaymen

password aymen/Hem!2020

- Avoir le status des process Gitlab
```
sudo gitlab-ctl status
```
- Editer le fichier /etc/gitlab/gitlab.rb
- set the external_url variable to the right hostname
- run the folowing command to reload the conf
```
sudo gitlab-ctl reconfigure
```
