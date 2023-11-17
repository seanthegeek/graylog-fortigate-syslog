# Changelog

## 1.3.4-rev15

- Remove duplicate stream

## 1.3.4-rev13

- Add `applist` column to the Details table in the Application Control tab
- Add `profile` column to the Details table in the DNS Filter tab
- Add `policyname` column to the Details table in the Forward Traffic tab
- Add `profile` column to the Details table in the IPS tab
- Add `policyname` column to the Details table in the Multicast Traffic tab
- Add `profile` column to the Details table in the SSL/TLS/SSH Inspection tab
- Add `profile` column to the Details table in the Web Filter tab

## 1.3.3-rev12

- Actually include changes that were not saved in 1.3.2-rev11
  - Rename the FortiGate dashboard to FortiGate Syslog
  - Sort the dashboard pages again (hopefully the order sticks this time)
  - Update the content pack description/README
- IPS dashboard page fixes
  - Change the time range of the Severity widget from 30 days to 7 days to match the rest of the widgets
  - Rename Untitled Message table to Details

## 1.3.2-rev11

- Rename the FortiGate dashboard to FortiGate Syslog
- Sort the dashboard pages again (hopefully the order sticks this time)
- Fix dashboard typos
- Update the content pack description/README

## 1.3.1-rev10

- Update FortiGate Syslog Stream rule regex to include more formats of FortiGate serial numbers

## 1.3.0-rev9

- Fix install failures (issue #1)

## ## 1.2.1-rev8

- Fix the order of the dashboard tabs

## 1.2.0-rev7

- Remove duplicate streams from the content pack
- Add `user` field as a column in each Details table
- Add `catdesc` field in Web Filter Details table

## 1.1.0-rev4

- Add missing Details event table to the VPN dashboard page
- Fix dashboard bug in the Forward Traffic and Local traffic pages where sources would not be listed if the `srcmac` or `srcname` fields were missing from the log message

## 1.0.1-rev3

- Add Attack Destination IP Addresses widget to the IPS dashboard

## 1.0.0-rev1

- Initial release
