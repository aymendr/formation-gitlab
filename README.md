# formation-gitlab

## Installation
- Suivre le lien suivant pour l'installation : https://about.gitlab.com/install/#ubuntu


Installation:

# 1. Install and configure the necessary dependencies
```
sudo apt-get update
sudo apt-get install -y curl openssh-server ca-certificates tzdata perl
```
# install Postfix
```
sudo apt-get install -y postfix
```
# Add the GitLab package repository and install the package
```
curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh | sudo bash
```
# Next, install the GitLab package
```
sudo EXTERNAL_URL="http://gitlab.example.com" apt-get install gitlab-ee
```
# Add gitlab.example.com to your /etc/hosts next to 127.0.0.1
```
connect from your browser to http://gitlab.example.com
```
# Browse to the hostname and login
```/etc/gitlab/initial_root_password```. Use this password with username root to login.


password reset to root / aymenaymen

password aymen/Hem!2020
