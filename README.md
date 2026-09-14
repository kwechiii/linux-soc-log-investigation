# Linux SOC Log Investigation

## Overview
This project demonstrates a basic SOC investigation using Linux command-line
tools to identify, filter, correlate, and assess potentially suspicious
system events.

## Objectives
- Analyze Linux system logs for suspicious activity
- Identify failed and login-related events
- Correlate events using timestamps
- Perform basic security event triage
- Document investigation findings

## Tools Used
- Kali Linux
- Linux CLI
- grep
- cut
- sort
- uniq
- nano

## Investigation

Initial analysis identified:

- 5 events containing "failed"
- 3 login-related events
- 18 session-related events
- 0 SSH events
- 0 sudo events
- 0 explicit authentication-related events

Four failed events and three login-related events occurred around 13:00:47,
making this timestamp the primary event cluster investigated.

Further correlation of session activity showed multiple system sessions
throughout the investigation period.

## Assessment

The reviewed evidence did not provide sufficient indicators to classify the
activity as a confirmed security incident.

The investigation demonstrated the importance of correlating multiple log
events instead of treating individual keywords such as "failed" as proof of
malicious activity.

## Skills Demonstrated
- Linux log analysis
- SOC event triage
- Event correlation
- Timestamp analysis
- Command-line log filtering
- Incident documentation
