# Definition

A connection is an object that links two servers, allowing them to exchange data. It can be defined as  `SOURCE_IP:SOURCE_PORT>DESTINATION_IP:DESTINATION_PORT|CONNECTION_TYPE`.

Any remote interaction or communication between two or more servers relies on connections.

It is possible, and actually common, to multiple connections coexist among two servers.

# Packets

Every data flowing from servers over the Internet is presented as Network Packets. Those packets contain meaningful information about the performed action, including connection type, ports, IP addresses and action-specific data.

Some connections send encrypted packets by default, others don't. It is possible to encrypt an unsafe connection by using Encrypt.

Packets are generated in real time and can be eavesdropped with Fireshark. Unencrypted packets can contain sensitive data in plain-text, proving valuable to an attacker.

# Types

The connection type identifies the purpose of a given connection.

Usually, `DESTINATION_PORT` alone suffices to identify the type of a connection, but some types allows for multiple or random destination ports.

Below is a breakdown of the connection types.

## SSH

A `Secure Shell (SSH)` connection is opened when a user successfully logins to a remote computer. It allows the user to retrieve all information he has access to. If the user has `root` access, it means he has access to all data and software inside that server.

An SSH connection will exist for the duration of the remote access.

SSH connections are identified by port `22`.

## FTP

A `File Transfer Protocol (FTP)` connection is created whenever a user downloads or uploads a software to a remote server.

An FTP connection will exist for the duration of the file transfer, being automatically deleted when the transfer completes. 

FTP connections are identified by port `21`

## X11

The X11 connection exchanges graphical data between two servers. It allows a client to see the Desktop (Graphical User Interface) from the server, exactly as it is seem by the remote server. This includes open applications[HEPNOTE:note-privacy-x11] and potentially sensitive information.

A X11 connection starts when the client is using a Desktop/Web interface and is connected through an SSH connection. It is terminated at the end of the SSH session. 

X11 connections are identified by port `6000`.

## HTTP

The `Hypertext Transfer Protocol (HTTP)` connection sends website data from the server to the client. 

It is insecure in the sense that all data transferred from the server to the client can be read by potential hackers eavesdropping the network.

An HTTP connection starts when the client accesses a remote website and terminates a few seconds later, when the request has been fulfilled. 

HTTP connections are identified by port `80`.

## HTTPS

The `HTTP Secure (HTTPS)` connection is similar to `HTTP`, since it allows clients to request website data, but it encrypts all network packets exchanged between them.

HTTPS connections are identified by port `443`.

## Tor

Tor connections are identified by port `9001`.

## Proxy

The `Proxy` connection forwards the packets from the source to a third server. It is specially useful when an attacker wishes to hide his real IP address, or to complicate the action of tracing him down.

Proxy connections are identified by port `1080`.

## CRC

The `Cracker (CRC)` connection is established when an attacker is attempting a brute-force attack over a remote server.

The CRC connection terminates right after the password is obtained.

CRC connections are identified by port `TODO`.

## DDoS

The `DDoS` connection is a special type that identifies automatic attacks coming from botnets.

DDoS connections are identified by port `666`.

## Adware

## Torrent

Torrent connections are identified by port `6881`.

## Wire Transfer

A `Wire Transfer` connection happens between banks, allowing them to move money from one bank to another.

A Wire Transfer starts when someone starts a money transfer operation. This connection will be terminated when the transfer is done. The time to transfer the money depends mainly on the amount being transferred.

Wire Transfer connections are identified by port `TODO`.

## BTC

A `Bitcoin (BTC)` connection happens when a transaction block is being verified. The time to solve that block depends on how much money is being moved.

BTC connections are identified by port `8333`.

## DNS

DNS connections are identified by port `53`.

## BGP

BGP connections are identified by port `179`.

# Notes

[HEPNOTE:note-privacy-x11]: Applications that include real user personal data, or chat information, are not replicated. Examples include Settings, Billing, Chat and Email windows.