# playbook-includes
    test case for relative playbook includes with relative vars_files includes

https://github.com/ansible/ansible/issues/19398

```
.
├── playbooks
│   ├── bar.yml
│   ├── deploy
│   │   ├── baz.yml
│   │   └── foo.yml
│   ├── includes
│   │   └── myvars.yml
│   └── total-deploy.yml
```

Execute:

```
ansible-playbook -i localhost, --list-tags playbooks/total-deploy.yml 
```
