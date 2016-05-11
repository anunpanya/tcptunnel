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

$ git clone https://github.com/anunpanya/tcptunnel.git
$ cd tcptunnel
```

## Configure

```
nano tcptunnel.cfg

# host:domain name or ip address
# local port:remote port

host:example.com
80:80
443:443

```

## Run script

```
chmod +x start-tcptunnel
chmod +x stop-tcptunnel

./start-tcptunnel
echo "=================================================="
echo "                 TCPTunnel script"
echo "=================================================="
example.com
    127.0.0.1:80 <--> example.com:80
    127.0.0.1:443 <--> example.com:443
    
./stop-tcptunnel
Killed
```
