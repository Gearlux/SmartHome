# Better logging

Since a couple of days, my homeassistant server on the Raspberry Pi 4 stops responding.
The logs are deleted after restart, so I have no idea what is causing the problem.

In this [feature request](https://community.home-assistant.io/t/better-logging/185694/8), a solution is proposed to inspect the logging before a restart.

[comment]: # (I have no idea if the following fragment works. I could not find eventlog.csv)
In configuration.yaml
```
notify:
  - platform: file
    name: eventlog
    filename: eventlog.csv
    timestamp: true
```