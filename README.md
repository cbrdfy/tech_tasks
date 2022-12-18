## Ansible playbook for python web app & PostgreSQL DB deployment

Python web app backend is based on:
- Python3
- Flask
- Gunicorn
- Nginx

PostgreSQL playbook is installing necessary packages and creating a database named __test_db__ and user __vagrant__. Password is encrypted by ansible-vault. Vault password is stored in _.vault_pass_ file.

### To deploy python web app and PostgreSQL DB run
```
ansible-playbook playbook.yml --vault-password-file .vault_pass
```

PostgreSQL playbook is installing necessary packages and creating a database named __test_db__ and user __vagrant__. Password is encrypted by ansible-vault. Vault password is stored in _.vault_pass_ file.

Testing was made on ubuntu 20.04 (vagrant box __generic/ubuntu2004__).
