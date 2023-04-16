# graylog-fortigate-syslog
A Graylog Content Pack of dashboards for FortiGate syslog data

## Setup

A complete guide can be found on [my blog][blog]. It explains how to create a single-node Graylog instance, import this Content pack, and configure FortiGate firewalls to send logs to the Graylog server.

## Streams

In Graylog, a stream routes log data to a specific index based on rules. This Content Pack includes one stream.

### FortiGate Syslog

The FortiGate Syslog stream includes a rule that matches all logs with a field named `devid` that has a value that starts with `FGT`, which is the beginning of every FortiGate seral number, and is included in every FordiGate log message.

## Dashboards

### FortiGate

The fortiGate dashboard has multiple pages. Each page contains a collection of dashboard widgets releated to a specific type of log data.

- Overview
- Application Control
- DNS Filter
- Forward Traffic
- IPS
- Local Traffic
- Multicast Traffic
- SSL/TLS/SSH Inspection
- VPN
- Web Filter


[blog]: https://seanthegeek.net/1270/how-to-create-a-single-node-graylog-instance-and-analyze-fortigate-logs/
