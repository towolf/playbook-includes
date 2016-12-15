# playbook-includes
    test case for relative playbook includes with relative vars_files includes

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
