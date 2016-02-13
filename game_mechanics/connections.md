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