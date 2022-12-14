# Sigma Network
Scripts to stand-up Home Network (Codenamed: Sigma).

## Packages to install
* Grafana
* Prometheus
* Ansible

## Setup SSH
May need to adjust /etc/ssh/sshd_config to allow Ansible Playbooks to run properly

`sudo vim /etc/ssh/sshd_config`

```
# To disable tunneled clear text passwords, change to no here!
PasswordAuthentication yes
#PermitEmptyPasswords no

# Change to yes to enable challenge-response passwords (beware issues with
# some PAM modules and threads)
ChallengeResponseAuthentication no
```

## Grafana Setup - v9.3.1

* Ubuntu & Debian

```
sudo apt-get install -y adduser libfontconfig1
wget https://dl.grafana.com/oss/release/grafana_9.3.1_amd64.deb
sudo dpkg -i grafana_9.3.1_amd64.deb
```

## Prometheus Setup - v2.40.7

```
wget https://github.com/prometheus/prometheus/releases/download/v2.40.7/prometheus-2.40.7.linux-amd64.tar.gz
tar xvf prometheus-2.40.6.linux-amd64.tar.gz
```
