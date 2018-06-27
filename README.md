# Kenken POC ansible Playbook

## Ansible

### Install ansible

Mac OS

```bash
brew install ansible
```

### Run ansible

```bash
ansible-playbook -u ec2-user -i hosts setup.yml --private-key=/path/to/${KEY_FILE}
```

*append logrotate configuration files*

## Serverspec

### Install serverspec

```bash
gem install serverspec
```

### Run serverspec

```bash
# you have to set `section` in ENV
export section=api-staging

# and you can run rake task
rake
```

avaiable section is below.

- api-staging
- api-production
