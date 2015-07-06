# How to Deploy J2EE
## Getting Started

First ensure you have JDK version '1.7' or higher:

```bash 
$ java -version 
1.7
```

Then, install the following items:
1. GlassFish 4.1
2. MySql



## Run Kitty Run

Both `MySql` and `GlassFish` have a sets of command utilities for user to control their life-cycle:


### MYSQL

First start the server daemon (to run server-service in background):

```bash
$ mysql.server start 
```

Then, `mysql.server` will expose *tcp-port:3306* for `MySql` client to connect.


### GlassFish

To create new domain:

```bash 
$ sudo asadmin create-domain --adminport 4848 <your-domain-name>
```

To start domain: (admin authorization is required in Mac)

```
$ sudo asadmin start-domain <your-domain-name>
```

To stop domain: (remember to stop domain before you can configure glassfish at intellij)

```bash
$ asdamin stop-domain <your-domain-name>
```

 









