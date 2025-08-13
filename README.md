# Deployer automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-deployer
  name: ansible-role-deployer
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-deployer

- Import role and override role variables, e.g.
```
- name: Setup deployer
  roles:
    - role: ansible-role-deployer
```

- All available role vars can be found in `defaults`
