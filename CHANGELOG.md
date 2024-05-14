# Changelog

## 1.7.0-rev29

- Fix byte count dashboard widgets so they do not sum duplicate values

## 1.6.6-rev27

- Update `FortiGate Syslog` stream regex rule to cover VM serial numbers (PR #13)

## 1.6.5-rev26

- Remove `stream_title` object from the content pack

## 1.6.4-rev24

- Use `subtype:forward AND action:accept` as the filter query for the net flow widgets

## 1.6.3-rev23

- Filter out `action:start` in the Top 500 Sources widget in the Forward Traffic dashboard page

## 1.6.2-rev22

- Swap the positions of the Top 500 sources by Bytes and top 100 Destinations by Bytes widgets

## 1.6.1-rev22

- Add `subtype:forward` to the query for the Top 500 Applications by Bytes widget

## 1.6.0-rev21

- Add net flow widgets to the Forward Traffic dashboard page
  - Top 500 Applications by Bytes
  - Top 500 Destinations by Bytes
  - Top 500 Sources by Bytes

## 1.5.2-rev20

- Fix broken install
- Update `FortiGate Syslog` stream regex rule to cover more serial numbers (close #9)

## 1.5.1-rev19

- Revert stream name from `FortiGate syslog` back to `FortiGate Syslog` to resolve compatibility with existing installs

## 1.5.0-rev18

- Move the pipeline to a separate content pack because Graylog does not create the stream required stream included in the content pack before trying to install the pipeline that depends on the stream

## 1.4.2-rev-17

- Add `craction to long` and `incidentserialno to long` pipeline rules

## 1.4.1-rev16

- Do not remove the `sessionid` field

## 1.4.0-rev15

- Add `FortiGate syslog data cleanup` pipeline

## 1.3.4-rev14

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
