# graylog-fortigate-syslog

A Graylog Content Pack of dashboards for FortiGate syslog data

## Setup

A complete guide can be found on [my blog][blog]. It explains how to create a single-node Graylog instance, import this Content pack, and configure FortiGate firewalls to send logs to the Graylog server.

In Graylog, a stream routes log data to a specific index based on rules. This Content Pack includes one stream.

## FortiGate syslog stream

In Graylog, a stream routes log data to a specific index based on rules. This Content Pack includes one stream.

The FortiGate Syslog stream includes a rule that matches all logs with a field named `devid` that has a value that matches the regex pattern `^FG([0-9]{2,3})[A-Z]T|^FGT`, which is the beginning of every FortiGate seral number, and is included in every FortiGate log message.

## FortiGate syslog data cleanup pipeline

Converts FortiGate syslog fields to the correct data type and removes unnecessary fields.

## FortiGate syslog dashboard

The FortiGate Syslog dashboard has multiple pages. Each page contains a collection of dashboard widgets related to a specific type of log data.

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
