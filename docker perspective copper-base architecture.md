## Docker perspective copper-base architecture

#### In here we are trying to give some brief idea about, how copper-base behave in docker envirenment. 
#### Copper-base contains main 5 docker containers. Those are

  - Reverse proxy (C1)
  - Email server (C2)
  - LDAP (C3)
  - Webmail (C4)
  - Redis (5)
  
#### Diagram

![Octocat](https://github.com/LankaSoftwareFoundation/Copper-EmailSolution/blob/master/docker_perspective_copper_base_architecture.png)

#### 1 Reverse proxy

This is very important when accessing internal web application through a single point. It works as a reverse proxy for following web portals.
  1. web mail
  2. phpldapadmin
  3. agent

#### 2 Email server

Main container in the solution. It has Postfix (as SMTP server), Dovecot, mailbox, Rsapmd for spam filtering and Zeyple for encrypt the content of the emails.

#### 3 LDAP

This is the directory service and it holds user data. It works as the user management part of the copper email server. Admin user can access the LDAP data through "phpLDAPadmin" protal.

#### 4 Webmail

It contains webmail client for the soulution. Currently we run rainloop as the webmail client.

#### 5 Redis 

Redis is an open source, in-memory data structure store, used as a database, cache and message broker. It supports data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs and geospatial indexes with radius queries. Redis has built-in replication, Lua scripting, LRU eviction, transactions and different levels of on-disk persistence, and provides high availability via Redis Sentinel and automatic partitioning with Redis Cluster.
