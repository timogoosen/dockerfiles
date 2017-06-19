## BTCD in a container:

Run :

```

$ docker build -t btcd .


```

Start container and let it read from local ~/.btcd directory for config and read data for blocks etc also can write to logging directory.
Use Docker volumes for that part:


```
$ docker run e58ee15cbde5 --volume=~/.btcd/:/root/btcd/



```
