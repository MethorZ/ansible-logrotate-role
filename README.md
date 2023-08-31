ansible-logrotate-role
=========

Ansible role to perform log rotation

Requirements
------------

None

Role Variables
--------------
```YAML
# Enable log rotation role
logrotate_enabled: false

# Configure log rotations
logrotate_configurations: []
#  # Example setup
#  - name: my-logs
#    files:
#      - /var/log/my-log-file.log
#      - /var/log/news/*
#    frequency: daily # yearly | monthly | weekly | daily | hourly (requires crontab modification)
#    rotation: 5
#    compress: true
#    create_mode: 644 root root
#    rotate_if_empty: true
#    ignore_missing_log_error: false
```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: methorz.logrotate }

License
-------

BSD

Author Information
------------------

https://twitter.com/methor_z
