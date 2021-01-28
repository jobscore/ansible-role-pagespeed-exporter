[![Build Status](https://travis-ci.org/jobscore/ansible-role-pagespeed-exporter.svg?branch=master)](https://travis-ci.org/github/jobscore/ansible-role-pagespeed-exporter)

Prometheus Pagespeed Exporter role
=========

An Ansible role for installing Prometheus Pagespeed Exporter on a Ubuntu box.
This role is based on https://github.com/jobscore/pagespeed_exporter

Requirements
------------

Pagespeed api key.

Role Variables
--------------

```
prometheus_pagespeed_port: The port in which the exporter will expose the metrics. Default to 9271
prometheus_pagespeed_version: Version of the exporter. Default to 2.1.2
prometheus_pagespeed_api_key: Pagespeed api key
prometheus_pagespeed_targets: Comma separated list of targets to inspect. Required
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - role: jobscore.prometheus_passenger_exporter
          prometheus_pagespeed_api_key: <api_key>
          prometheus_pagespeed_targets: https://google.com

License
-------

[MIT](/LICENSE)

Author Information
------------------

This role was created by [GlauberrBatista](https://github.com/GlauberrBatista) while working for [JobScore Inc](https://jobscore.com).
