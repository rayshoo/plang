# Env

## How to use
1. [Install ansible package](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

2. Specifies the role to be performed in [site.yaml](site.yaml)
```yaml
# site.yaml
---
roles:
  - golang
  - nodejs
```

3. Type the version of golang you want to install in [site.yaml](site.yaml)

```yaml
# site.yaml
---
vars:
  version:
    golang: 1.17
    nodejs: 14.17.5
```

4. Set the host to be executed in [hosts.ini](hosts.ini) and [site.yaml](site.yaml)

5. run the playbook
```sh
$ ansible-playbook site.yaml
```
