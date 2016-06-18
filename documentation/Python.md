# Python

```sh
root@edison:~# python
Python 2.7.11 (default, Apr 28 2016, 00:50:26) 
[GCC 5.3.0] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

```sh
root@edison:~# git clone https://github.com/xe1gyq/TheIoTLearningInitiative.git
Cloning into 'TheIoTLearningInitiative'...
remote: Counting objects: 75, done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 75 (delta 1), reused 0 (delta 0), pack-reused 68
Unpacking objects: 100% (75/75), done.
Checking connectivity... done.
root@edison:~# 
```

```
root@edison:~# cd TheIoTLearningInitiative/
root@edison:~/TheIoTLearningInitiative# ls
InternetOfThings101  LICENSE              README.md
root@edison:~/TheIoTLearningInitiative# cd InternetOfThings101/
root@edison:~/TheIoTLearningInitiative/InternetOfThings101# ls
README.md            main.py              requirements.manual  requirements.pip
root@edison:~/TheIoTLearningInitiative/InternetOfThings101# python main.py 
Traceback (most recent call last):
  File "main.py", line 3, in <module>
    import paho.mqtt.client as paho
ImportError: No module named paho.mqtt.client
root@edison:~/TheIoTLearningInitiative/InternetOfThings101# pip install -r requirements.pip            
Collecting psutil (from -r requirements.pip (line 1))
...
error: command 'i686-ostro-linux-gcc' failed with exit status 1
...
```

Install libz-dev, how?!

```sh
root@edison:~/TheIoTLearningInitiative/InternetOfThings101# cat requirements.manual 
wget https://launchpad.net/python-weather-api/trunk/0.3.8/+download/pywapi-0.3.8.tar.gz
tar zxvf pywapi-0.3.8.tar.gz
cd pywapi-0.3.8
python setup.py build
python setup.py install
cd ..
rm -rf pywapi-0.3.8*
root@edison:~/TheIoTLearningInitiative/InternetOfThings101# sh requirements.manual 
```

```
root@edison:~/TheIoTLearningInitiative/InternetOfThings101# pip install paho-mqtt
Collecting paho-mqtt                     
Installing collected packages: paho-mqtt
Successfully installed paho-mqtt-1.2     
root@edison:~/TheIoTLearningInitiative/InternetOfThings101# 
```

```sh
root@edison:~/TheIoTLearningInitiative# git clone https://github.com/giampaolo/psutil.git
Cloning into 'psutil'...
remote: Counting objects: 18500, done.
remote: Compressing objects: 100% (113/113), done.
remote: Total 18500 (delta 66), reused 0 (delta 0), pack-reused 18387
Receiving objects: 100% (18500/18500), 25.74 MiB | 1.09 MiB/s, done.
Resolving deltas: 100% (13230/13230), done.
Checking connectivity... done.
root@edison:~/TheIoTLearningInitiative# ls     
InternetOfThings101  LICENSE              README.md            psutil
root@edison:~/TheIoTLearningInitiative# cd psutil/
root@edison:~/TheIoTLearningInitiative/psutil# ls
CREDITS       IDEAS         MANIFEST.in   appveyor.yml  psutil        tox.ini
DEVGUIDE.rst  INSTALL.rst   Makefile      docs          scripts
HISTORY.rst   LICENSE       README.rst    make.bat      setup.py
root@edison:~/TheIoTLearningInitiative/psutil# python setup.py install
running install
running bdist_egg
running egg_info
creating psutil.egg-info
writing psutil.egg-info/PKG-INFO
writing top-level names to psutil.egg-info/top_level.txt                                               
writing dependency_links to psutil.egg-info/dependency_links.txt                                       
writing manifest file 'psutil.egg-info/SOURCES.txt'                                                    
reading manifest file 'psutil.egg-info/SOURCES.txt'                                                    
reading manifest template 'MANIFEST.in'                                                                
warning: no previously-included files matching '*' found under directory 'docs/_build'                 
writing manifest file 'psutil.egg-info/SOURCES.txt'                                                    
installing library code to build/bdist.linux-i686/egg                                                  
running install_lib                                                                                    
running build_py                                                                                       
creating build                                                                                         
creating build/lib.linux-i686-2.7                                                                      
creating build/lib.linux-i686-2.7/psutil                                                               
copying psutil/_pswindows.py -> build/lib.linux-i686-2.7/psutil                                        
copying psutil/__init__.py -> build/lib.linux-i686-2.7/psutil                                          
copying psutil/_pssunos.py -> build/lib.linux-i686-2.7/psutil                                          
copying psutil/_common.py -> build/lib.linux-i686-2.7/psutil                                           
copying psutil/_psbsd.py -> build/lib.linux-i686-2.7/psutil                                            
copying psutil/_psosx.py -> build/lib.linux-i686-2.7/psutil                                            
copying psutil/_pslinux.py -> build/lib.linux-i686-2.7/psutil                                          
copying psutil/_psposix.py -> build/lib.linux-i686-2.7/psutil                                          
copying psutil/_compat.py -> build/lib.linux-i686-2.7/psutil                                           
creating build/lib.linux-i686-2.7/psutil/tests                                                         
copying psutil/tests/__init__.py -> build/lib.linux-i686-2.7/psutil/tests                              
copying psutil/tests/test_process.py -> build/lib.linux-i686-2.7/psutil/tests                          
copying psutil/tests/test_osx.py -> build/lib.linux-i686-2.7/psutil/tests                              
copying psutil/tests/test_sunos.py -> build/lib.linux-i686-2.7/psutil/tests                            
copying psutil/tests/test_linux.py -> build/lib.linux-i686-2.7/psutil/tests                            
copying psutil/tests/test_posix.py -> build/lib.linux-i686-2.7/psutil/tests                            
copying psutil/tests/test_windows.py -> build/lib.linux-i686-2.7/psutil/tests                          
copying psutil/tests/test_misc.py -> build/lib.linux-i686-2.7/psutil/tests                             
copying psutil/tests/test_bsd.py -> build/lib.linux-i686-2.7/psutil/tests                              
copying psutil/tests/test_memory_leaks.py -> build/lib.linux-i686-2.7/psutil/tests                     
copying psutil/tests/test_system.py -> build/lib.linux-i686-2.7/psutil/tests                           
copying psutil/tests/runner.py -> build/lib.linux-i686-2.7/psutil/tests                                
running build_ext                                                                                      
building 'psutil._psutil_linux' extension                                                              
creating build/temp.linux-i686-2.7                                                                     
creating build/temp.linux-i686-2.7/psutil                                                              
i686-ostro-linux-gcc -m32 -march=atom -msse3 -mfpmath=sse -fno-strict-aliasing -O2 -pipe -g -feliminate
-unused-debug-types -fdebug-prefix-map=/var/lib/jenkins/ostro-worker-16-slot-1-E6DRp/ostro-os/build/tmp
-glibc/work/edison-ostro-linux/python/2.7.11-r1=/usr/src/debug/python/2.7.11-r1 -fdebug-prefix-map=/var
/lib/jenkins/ostro-worker-16-slot-1-E6DRp/ostro-os/build/tmp-glibc/sysroots/x86_64-linux= -fdebug-prefi
x-map=/var/lib/jenkins/ostro-worker-16-slot-1-E6DRp/ostro-os/build/tmp-glibc/sysroots/edison= -fstack-p
rotector-strong -D_FORTIFY_SOURCE=2 -Wformat -Wformat-security -DNDEBUG -g -O3 -Wall -Wstrict-prototype
s -fPIC -DPSUTIL_VERSION=430 -I/usr/include/python2.7 -c psutil/_psutil_linux.c -o build/temp.linux-i68
6-2.7/psutil/_psutil_linux.o                                                                           
i686-ostro-linux-gcc -m32 -march=atom -msse3 -mfpmath=sse -shared -Wl,-O1 -Wl,--hash-style=gnu -Wl,--as
-needed -fstack-protector-strong -Wl,-z,relro,-z,now build/temp.linux-i686-2.7/psutil/_psutil_linux.o -
L/usr/lib -lpython2.7 -o build/lib.linux-i686-2.7/psutil/_psutil_linux.so                              
/usr/lib/gcc/i686-ostro-linux/5.3.0/../../../../i686-ostro-linux/bin/ld: cannot find -lssp_nonshared   
/usr/lib/gcc/i686-ostro-linux/5.3.0/../../../../i686-ostro-linux/bin/ld: cannot find -lssp             
collect2: error: ld returned 1 exit status                                                             
error: command 'i686-ostro-linux-gcc' failed with exit status 1                                        
root@edison:~/TheIoTLearningInitiative/psutil# 
```

```sh
root@edison:~# wget http://mirrors-usa.go-parts.com/gcc/releases/gcc-5.3.0/gcc-5.3.0.tar.bz2
--2016-06-18 10:02:41--  http://mirrors-usa.go-parts.com/gcc/releases/gcc-5.3.0/gcc-5.3.0.tar.bz2
Resolving mirrors-usa.go-parts.com... 68.233.45.189
Connecting to mirrors-usa.go-parts.com|68.233.45.189|:80... connected.
HTTP request sent, awaiting response... 200 OK
Length: 95441837 (91M) [application/octet-stream]
Saving to: 'gcc-5.3.0.tar.bz2'

gcc-5.3.0.tar.bz2         100%[====================================>]  91.02M   477KB/s    in 2m 42s  

2016-06-18 10:05:24 (575 KB/s) - 'gcc-5.3.0.tar.bz2' saved [95441837/95441837]

root@edison:~# tar xvf gcc-5.3.0.tar.bz2 

```