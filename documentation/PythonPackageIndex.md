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
