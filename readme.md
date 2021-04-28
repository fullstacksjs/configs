# Fulstacks configs

## ansible

requirments

- ansible
- python3

### how to run ?

```sh
ansible-playbook path-to-play-file.yml
```

**include :**

### i - prepare-ubuntu

install and configure

- nginx
- python
- curl
- git
- config firewall (ufw)

### ii - register github ci runner

set a github actions runner on your machine.
variables:
var name | var val
------------- | -------------
DOCKER_USERNAME | your docker hub username
DOCKER_PASS| your docker hub password
CI_CODE| your ci hash ( from github/repo setting/actions/set new)
CI_PATH| repository url
CI_NAME| your ci name
