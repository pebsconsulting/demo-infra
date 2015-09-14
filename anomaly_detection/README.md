# mPlane Anomaly detection component and reasoner

This module contains anomaly detection component and reasoner developed utilizing mPlane SDK.




Please be aware that THIS IS A BETA VERSION, MAY CONTAIN SOME BUGS.

## Reasoner
The __mpadtoolreasoner__ is a Python script based on __mpcli__ and extended to run reasoning tasks triggered by __adtool.pl__ .

##Supervisor

Supervisor udsed is the one provided by mPlane SDK.

##Howto

Follow these steps to run the use case.

1. Set parameters for supervisor.conf, adtool.conf, client.conf please use mPlane docs on how to set parameters in configuration files.
2. Run supervisor, open new terminal, enter protocol-ri, and execute:
```
$ export PYTHONPATH=.
$ ./scripts/mpsup --config ./conf/supervisor.conf
```
3. Run adtool component proxy:
Open a new terminal, enter __protocol-ri__ folder and execute:

```
$ export PYTHONPATH=.
$ ./scripts/mpcom --config ./mplane/components/ADTool/conf/adtool.conf

```

4. Run reasoner:

```
$ export PYTHONPATH=.
$ ./scripts/mpadtoolreasoner --config ./conf/client.conf

```

