# install sql with playbook

```ansible

---
# installing Mysql on a server called db

- hosts: db
  become: true
  tasks:
  - name: Install mysql
    apt: pkg=mysql-server state=present
```