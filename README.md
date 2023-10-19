# Configuration
Stored in fftp.conf file, contain configuration section named ftpconfig and number of sections describing users and their privileges.
[ftpconfig]

  port

Port number to bind the server to. Default: 21

  maxusers

Maximum connections count to the server, that can be established simultaneously. Default: 1

  interface

Interface IP to bind to. Use 0.0.0.0 to listen on any available interface. Default: 127.0.0.1

  external_ip

If you running the server behind a NAT, it is a good idea to put your real IP here. This will help clients to establish data connections. Default: 0.0.0.0

  local_mask

IP mask for local network. This will help the server to distinguish between local and Internet clients. Default: 255.255.255.0

  minport
  maxport

Port range for data connections. You can use it to configurate port forwarding on your gateway device. Default: 1024..65535

  logfilepath

Full path with file name for a log file. Comment or delete it to disable logging. Default: disabled

  CATrustFile

It is recommended to leave this option as it is (/etc/ssl/certs/ca-certificates.crt)

  ServerCertificate

Path to your SSL certificate. Accepted format is x509 ASCII PEM.

  Keyfile

Path to PEM private key file for your certificate.

  KeyfilePassword

Password to decrypt private key.

  keepalive

Send keepalive packets (some NATs may require this). Default: 0 (disabled)
