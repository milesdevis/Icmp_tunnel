#Installation

Download repo and run `make` on client and server 

On server run the tunnel, the following: 
 ```
 ./icmptunnel -s 10.0.1.1
```

On the client, find gateway and its NIC, then go to client.sh:
replace \<server> with the IP address of the proxy server, \<gateway> with gateway address
Make sure your DNS server can access the proxy

Run the tunnel on the client: 
```
./icmptunnel -c <server>
```
The client should now be able to access the internet.
