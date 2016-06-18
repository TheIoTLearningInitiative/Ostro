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
root@edison:~# ls
get-pip.py  pip                            
root@edison:~# python get-pip.py
root@edison:~# python get-pip.py
Collecting pip
  Downloading pip-8.1.2-py2.py3-none-any.whl (1.2MB)
    100% |################################| 1.2MB 77kB/s
Collecting wheel
  Downloading wheel-0.29.0-py2.py3-none-any.whl (66kB)
    100% |################################| 71kB 484kB/s   
Installing collected packages: pip, wheel
Successfully installed pip-8.1.2 wheel-0.29.0              
root@edison:~# easy_install pip
```

```sh
root@edison:~# easy_install requests
Searching for requests
Reading https://pypi.python.org/simple/requests/
Best match: requests 2.10.0
Downloading https://pypi.python.org/packages/49/6f/183063f01aae1e025cf0130772b55848750a2f3a89bfa11b385b
35d7329d/requests-2.10.0.tar.gz#md5=a36f7a64600f1bfec4d55ae021d232ae
Processing requests-2.10.0.tar.gz
Writing /tmp/easy_install-E4KeMV/requests-2.10.0/setup.cfg
Running requests-2.10.0/setup.py -q bdist_egg --dist-dir /tmp/easy_install-E4KeMV/requests-2.10.0/egg-d
ist-tmp-qSTGq5
warning: no files found matching 'test_requests.py'
creating /usr/lib/python2.7/site-packages/requests-2.10.0-py2.7.egg
Extracting requests-2.10.0-py2.7.egg to /usr/lib/python2.7/site-packages
Adding requests 2.10.0 to easy-install.pth file

Installed /usr/lib/python2.7/site-packages/requests-2.10.0-py2.7.egg
Processing dependencies for requests
Finished processing dependencies for requests
root@edison:~# 
```
