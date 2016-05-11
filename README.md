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

host:s1.example.com
80:80
443:443

host:s2.example.com
81:81
8080:8080
```

## Run script

```
chmod +x start-tcptunnel
chmod +x stop-tcptunnel

./start-tcptunnel
echo "=================================================="
echo "                 TCPTunnel script"
echo "=================================================="
s1.example.com
    127.0.0.1:80 <--> s1.example.com:80
    127.0.0.1:443 <--> s1.example.com:443
s2.example.com
    127.0.0.1:81 <--> s2.example.com:81
    127.0.0.1:8080 <--> s2.example.com:8080
    
./stop-tcptunnel
Killed
```
