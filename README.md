# Resque web Playbook

- install roles

```
ansible-galaxy install -r requirements.yml -p roles
```

- install resque web

```
ansible-playbook -i hosts.{stagefile} site.yml
```


