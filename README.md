[![Build Status](https://www.travis-ci.org/securCom/ansible-role_repo-mariadb.svg?branch=master)](https://www.travis-ci.org/securCom/ansible-role_repo-mariadb)
[![GitHub release](https://img.shields.io/github/release/securCom/ansible-role_repo-mariadb.svg)](https://github.com/securCom/ansible-role_repo-mariadb)


# Repo: MariaDB

Manage MariaDB  repositories.

# Requirements

For supported systems  see https://downloads.mariadb.org/mariadb/repositories/. If yhour system is not supported,
the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `mariadb_repo_version`: the mariadb version to install
- `mariadb_repo_state`: define presence of the repository
- `mariadb_repo_debian_mirror`: mirror for Debian/Ubuntu distribitions

# Dependencies

There no external dependencies.

# Example Playbook

To install role, add following line to **ansible-galaxy** requirements file
```
- src: https://github.com/securCom/ansible-role_repo-mariadb
  version: master
  name: securcom.repo_mariadb
```

```
- hosts: servers
  roles:
     - securcom.repo_mariadb
```

For list of packages see the documentation https://mariadb.com/kb/en/library/binary-packages/

- 
# License

BSD

# Author Information


- Peter Hudec (@hudecof)