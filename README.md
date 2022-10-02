## Python web app
### To deploy python web app run
```
ansible-playbook app_playbook.yml
```
Python web app backend is based on:
- Python3
- Flask
- Gunicorn
- Nginx

## PostgreSQL DB deployment
### To deploy postgresql db run
```
ansible-playbook postgresql_playbook.yml --vault-password-file .vault_pass
```
PostgreSQL playbook is installing necessary packages and creating a database named __test_db__ and user __vagrant__. Password is encrypted by ansible-vault. Vault password is stored in _.vault_pass_ file.
