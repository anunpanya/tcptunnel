# tcptunnel
bash shell script tcptunnel

Tcptunnel is a simple TCP port forwarder. Please see http://www.vakuumverpackt.de/tcptunnel/ for details and binary downloads.

##Install tcptunnel
### For Unix

```
$ git clone https://github.com/vakuum/tcptunnel.git
$ cd tcptunnel
$ ./configure
$ make
$ make install
```

### Configure

```
nano tcptunnel.cfg

# host:domain name or ip address
# local port:remote port

host:example.com
80:80
443:443

```

### Run script

```
./start-tcptunnel
```
