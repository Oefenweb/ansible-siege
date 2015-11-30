## siege

[![Build Status](https://travis-ci.org/Oefenweb/ansible-siege.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-siege) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-siege-blue.svg)](https://galaxy.ansible.com/list#/roles/5962)

Set up the latest version of [siege](https://www.joedog.org/siege-home/) in Debian-like systems.

#### Requirements

None

#### Variables

* `siege_remove_distro_version`: [default: `true`]: Whether or not to remove the distribution version

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - siege
```

#### License

MIT

#### Author Information

* Mark van Driel
* Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-siege/issues)!
