# prometheus_remote_write_users

Manage nginx htpasswd users allowed to write to the central Prometheus
remote-write endpoint.

```yaml
prometheus_remote_write_users:
  - name: 'collector_one'
    password: 'changeme'
    path: '/etc/nginx/htpasswd-prometheus'
    owner: 'root'
    group: 'www-data'
    mode: '0640'
```

Passwords should be stored with Ansible Vault.
