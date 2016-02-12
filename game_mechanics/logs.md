# Logs

## Overview

A log is a text entry containing details about an activity that happened on a server. Every recorded log is appended to a logfile.

A log entry can contain sensitive information, like someone's else IP address or bank account information, thus making it a vital part of the gameplay.

In order to cover their actions, attackers usually delete their logs. However, a deeper dynamic may be achieved by forging logs, thus deceiving or misleading someone to a honeypot or a third-party server.

## Tampering logs

Logs can be modified or deleted, but they can also be recovered!

An attacker wishing to clear any traces of his actions may choose to delete a log using the Log Forger. Another option would be to modify the log entry and point it to another server.

Any modification to a software can be undone with a Log Recover. The Software Version Dynamic plays an important role here.

Technically, a Log Recover 1.0 can undo *any* change made by *any* Log Forger. The catch, however, is that it may take several hours depending on the version delta. During that time, the person recovering the log is exposing herself by keeping an open connection.

The attacker can also hide a log using Hider. This can be undone by using Seeker;

Hiding a log entry adds a layer of protection against possible recovery, since someone else would have to first unhide the log, and then recover it.[TODO: does order matter?]

## Log Uncertainty

An interesting aspect of logs is that you can never know for sure if a given entry is a real one.

A single log entry can have several modifications, one after another, which will stack up.

Since Log Recover relies on an Iterative Process, every successful recovery pops a modification from the log stack. However, this is an endless process that can take very long to pop the next entry, so you can't be sure wheter you are seeing the real log.