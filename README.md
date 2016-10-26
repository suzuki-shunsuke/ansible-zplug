zplug
======

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-zplug.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-zplug)

Install [zplug](https://github.com/zplug/zplug).

Requirements
------------

* [motemen/ghq](https://github.com/motemen/ghq)

Role Variables
--------------

* ghq_executable: The executable path of ghq command. The default is "ghq".
* zplug_home: The directory zplug will store/load packages. The default is the environment variable "ZPLUG_HOME" or ~/.zplug .

Dependencies
------------

* [suzuki-shunsuke.ghq-module](https://galaxy.ansible.com/suzuki-shunsuke/ghq-module/)

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - suzuki-shunsuke.zplug
```

License
-------

MIT
