# Python Package Index


```sh
```

```sh
```

```sh
root@edison:~# curl --verbose -O https://bootstrap.pypa.io/get-pip.py
* getaddrinfo(3) failed for bootstrap.pypa.io:443
* Couldn't resolve host 'bootstrap.pypa.io'
* Closing connection 0
curl: (6) Couldn't resolve host 'bootstrap.pypa.io'
root@edison:~# 
```

```sh
root@edison:~# curl --verbose -O https://bootstrap.pypa.io/get-pip.py                                  
*   Trying 23.235.40.175...                                                                            
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current                        
                                 Dload  Upload   Total   Spent    Left  Speed                          
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* Connected to bootstrap.
pypa.io (23.235.40.175) port 443 (#0)                                                                  
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* found 173 certificates 
in /etc/ssl/certs/ca-certificates.crt                                                                  
* ALPN, offering http/1.1                                                                              
* SSL connection using TLS1.2 / ECDHE_RSA_AES_128_GCM_SHA256                                           
*        server certificate verification OK                                                            
*        server certificate status verification SKIPPED                                                
*        common name: *.c.ssl.fastly.net (matched)                                                     
*        server certificate expiration date OK                                                         
*        server certificate activation date OK                                                         
*        certificate public key: RSA                                                                   
*        certificate version: #3                                                                       
*        subject: C=US,ST=California,L=San Francisco,O=Fastly\, Inc.,CN=*.c.ssl.fastly.net             
*        start date: Fri, 22 Apr 2016 20:04:06 GMT                                                     
*        expire date: Sat, 29 Oct 2016 21:57:12 GMT                                                    
*        issuer: C=BE,O=GlobalSign nv-sa,CN=GlobalSign CloudSSL CA - SHA256 - G3                       
*        compression: NULL                                                                             
* ALPN, server accepted to use http/1.1                                                                
> GET /get-pip.py HTTP/1.1                   
> Host: bootstrap.pypa.io                    
> User-Agent: curl/7.47.1                                
> Accept: */*                                            
>                          
< HTTP/1.1 200 OK                              
< Server: nginx                
< Content-Type: text/x-python
< Last-Modified: Sat, 21 May 2016 23:30:29 GMT
< ETag: "5740ef95-1743f2"     
< X-Clacks-Overhead: GNU Terry Pratchett
< Strict-Transport-Security: max-age=315360000; includeSubDomains; preload                             
< Via: 1.1 varnish                   
< Content-Length: 1524722                       
< Accept-Ranges: bytes       
< Date: Sat, 18 Jun 2016 09:21:24 GMT
< Via: 1.1 varnish                                 
< Age: 5203
< Connection: keep-alive
< X-Served-By: cache-iad2120-IAD, cache-ord1734-ORD
< X-Cache: HIT, HIT                       
< X-Cache-Hits: 82, 21
<                          
{ [2264 bytes data]
100 1488k  100 1488k    0     0   279k      0  0:00:05  0:00:05 --:--:--  348k                         
* Connection #0 to host bootstrap.pypa.io left intact
root@edison:~# 

```

```sh
root@edison:~# easy_install pip                                                                        
Searching for pip                                                                                      
Reading https://pypi.python.org/simple/pip/                                                            
Download error on https://pypi.python.org/simple/pip/: [Errno -3] Temporary failure in name resolution!
Couldn't find index page for 'pip' (maybe misspelled?)                                                 
Scanning index of all packages (this may take a while)                                                 
Reading https://pypi.python.org/simple/                                                                
Download error on https://pypi.python.org/simple/: [Errno -3] Temporary failure in name resolution -- !
No local packages or download links found for pip                                                      
error: Could not find suitable distribution for Requirement.parse('pip')                               
root@edison:~# 
```

