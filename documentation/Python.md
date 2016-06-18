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