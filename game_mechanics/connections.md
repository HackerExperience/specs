# Connections

## Definition

A connection is an object that links two servers, allowing them to exchange data. It can be defined as  `SOURCE_IP:SOURCE_PORT/DESTINATION_IP:DESTINATION_PORT/CONNECTION_TYPE`.

Any remote interaction or communication between two or more servers relies on connections.

It is possible, and actually common, to multiple connections coexist among two servers.

## Types

The connection type identifies the purpose of a given connection.

Usually, `DESTINATION_PORT` alone suffices to identify the type of a connection, but some types allows for multiple or random destination ports.

Below is a breakdown of the connection types.

### SSH

A Secure Shell (SSH) connection is opened when a user successfully logins to a remote computer. It allows the user to retrieve all information he has access to. If the user has `root` access, it means he has access to all data and software inside that server.

An SSH connection will exist for the duration of the remote access and is identified by the port `22`.

### FTP

A File Transfer Protocol (FTP) connection is created whenever a user downloads or uploads a software to a remote server.

An FTP connection will exist for the duration of the file transfer, being automatically deleted when the transfer completes. It is identified by port `21`

### X11

The X11 connection exchanges graphical data between two servers. It allows a client to see the Desktop (Graphical User Interface) from the server, exactly as it is seem by the remote server. This includes open applications[HEPNOTE:note-privacy] and potentially sensitive information.

A X11 connection starts when the client is using a Desktop/Web interface and is connected through an SSH connection. It is terminated at the end of the SSH session. 

X11 connections are identified by port `6000` for the first client, `6001` for the second one and so on.

### HTTP

### HTTPS

### Tor

### CRC

### DDoS

### Adware

### Wire

### DNS

### BGP

## Packets

## Notes

[HEPNOTE:note-privacy]: Applications that include real user personal data, or chat information, are not replicated. Examples include Settings, Billing, Chat and Email windows.