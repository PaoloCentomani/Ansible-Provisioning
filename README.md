# Ansible Provisioning

1. Create a `hosts` file:

```ini
[webservers]
example_hostname ansible_host=123.123.123.123
```

2. Create a configuration file in `host_vars/example_hostname.yml`.

3. Run a playbook for a single host:

```bash
ansible-playbook -i hosts laravel.yml --limit example_hostname
```
