# Resque web Playbook

## install roles

```
ansible-galaxy install -r requirements.yml -p roles
```

## change config

please change configuration

- stage_vars/{stage}.yml

```
app_user: {resque_web exec username}
resque_web:
  config:
    host: {domain of the resque_web}
      redis:
        host: {ip of redis}
        port: {port of redis}
```

## install resque web

```
ansible-playbook -i hosts.{stagefile} site.yml
```

# exception clause
require operation. nginx restart in proxy server


