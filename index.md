---
layout: default
---

# Copper Email Solution


Copper Email Solution is a corporate email solution which can be used by any corporate organization and monitor and control from a central access point. It consists of 3 main parts as
1. Copper Base
2. Copper Suite
3. Copper Hub


## Copper Base

### Architecture

![Octocat](https://github.com/LankaSoftwareFoundation/Copper-EmailSolution/blob/master/mailServerArchitecture.png?raw=true)


#### Copper Base contains the email  soltions.

- [POSTFIX](http://www.postfix.org/) : a modular mail transfer agent.
- [DOVECOT](https://www.dovecot.org/) : secure open-source IMAP and POP3 server.
- [Rspamd](https://rspamd.com/) : spam filter.
- [RAINLOOP](https://www.rainloop.net/) : web client to access mail for users.
- [openldap](https://www.openldap.org/) : directory service which authenticate users.


## Contributors wellcome

Due to this is an opensource project contributors are welcome.
Copperbase readme file describe how to use this solution in development environments.
So any one who willing to contribute are wellcome and coppermail team is ready to support through their contacts.

https://github.com/LankaSoftwareFoundation/copper-base/blob/master/README.md

### Instruction for deployment (summary)

#### Create environment

1. Clone this Repository

```
$ git clone https://github.com/LankaSoftwareFoundation/copper-base.git
```

2. Edit .env file to replicate your settings

3. Create external Docker Network

```
$ docker network create front
$ docker network create back
```
#### Run

Run the system and start all services by :

```
$ docker-compose up -d 
```

#### You may join the copper mail group for updates.

- [Click me for check on mail group](https://groups.google.com/forum/#!forum/lsf-email-solution)
