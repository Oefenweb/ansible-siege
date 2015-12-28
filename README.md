## siege

[![Build Status](https://travis-ci.org/Oefenweb/ansible-siege.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-siege) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-siege-blue.svg)](https://galaxy.ansible.com/list#/roles/5962)

Set up the latest version of [siege](https://www.joedog.org/siege-home/) in Debian-like systems.

#### Requirements

None

#### Variables

* `siege_remove_distro_version`: [default: `true`]: Whether or not to remove the distribution version

* `siege_configuration_verbose`: [default: `true`]: Signify verbose mode
* `siege_configuration_quiet`: [default: `false`]: Quiet mode
* `siege_configuration_gmethod`: [default: `HEAD`]: Get method - select an HTTP method to use when siege is set to get mode (e.g. `GET`)
* `siege_configuration_limit`: [default: `255`]: This directive places a cap on the number of threads siege will generate
* `siege_configuration_show_logfile`: [default: `true`]: Show logfile location
* `siege_configuration_logging`: [default: `true`]: Default logging status
* `siege_configuration_protocol: [default: `HTTP/1.1`]: HTTP protocol (e.g. `HTTP/1.0`)
* `siege_configuration_chunked`: [default: `true`]: Chunked encoding is required by HTTP/1.1 protocol
* `siege_configuration_cache`: [default: `false`]: Cache revalidation
* `siege_configuration_connection`: [default: `close`]: Connection directive. (e.g. `keep-alive`)
* `siege_configuration_concurrent`: [default: `15`]: Default number of simulated concurrent users
* `siege_configuration_delay`: [default: `1`]: Default delay between each request by a single thread
* `siege_configuration_internet`: [default: `false`]: Internet simulation. If true, siege clients will hit the URLs in the urls.txt file randomly, thereby simulating internet usage
* `siege_configuration_benchmark`: [default: `false`]: Default benchmarking value, If true, there is NO delay between server requests, siege runs as fast as the web server and the network will let it
* `siege_configuration_accept_encoding`: [default: `gzip`]: Accept-encoding. This option allows you to specify acceptable encodings returned by the server
* `siege_configuration_url_escaping`: [default: `true`]: URL escaping was added in version 3.0.3. You may use this directive to turn off this experimental feature
* `siege_configuration_spinner`: [default: `true`]: TURN OFF THAT ANNOYING SPINNER!
* `siege_configuration_unique`: [default: `true`]: FTP unique - This directive determines whether siege will upload files with the same name

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
