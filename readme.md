# jæ's ghost deploy playbook

i made this for myself. it installs ghost, nginx, and sets up letsencrpt certificates

expected to run on ubuntu 16.04 (xenial)

## do it

1. `ansible-galaxy install -r requirements.yml`
2. copy `config.sample.yml` to `config.yml` and edit it as needed
    * definitely change `server_name` and `letsencrypt.email`
3. copy `hosts.sample` to `hosts` and update as needed
4. `ansible-playbook site.yml`
