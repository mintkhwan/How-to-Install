# How to install Sublime 2 & 3

## For Sublime-Text-2:
```
sudo add-apt-repository ppa:webupd8team/sublime-text-2
sudo apt-get update
sudo apt-get install sublime-text

```
## For Sublime-Text-3:
```
sudo add-apt-repository ppa:webupd8team/sublime-text-3
sudo apt-get update
sudo apt-get install sublime-text-installer

```


# How to install Package Control

### 1. เปิด sublime แล้วไปที่แถบด้านบน view show console
### 2.1   For sublime3
```
import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```
### 2.2   For sublime2
```
import urllib2,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')
```








# How to install Program or Package     #backend


### 1. Install NodeJS & npm
```
 sudo apt-get install curl
 curl --silent --location https://deb.nodesource.com/setup_4.x | sudo bash -
 sudo apt-get install nodejs
 sudo apt-get install npm
 
 check version -->   node -v
 check npm     -->   npm -v
```

### 2. Install ExpressJS
```
 npm init                       ---> create file package.json
 npm install express --save     ---> install package express make for server

```

### 3. Install http-server
```
 npm install http-server -g
 
```

### 4. Install Socketio
```
 npm init                              ---> create file package.json
 npm install --save express@4.10.2     ---> install package express make for server
 npm install --save socket.io          ---> install package socketio
```




# How to install MongoDB



### 1. install
```
 mkdir myproject                    ---> create folder project
 cd myproject
 mkdir data                         ---> create folder for database
 npm init
 npm install
 npm install mongodb                ---> create MongoDB
 npm install mongoose               ---> create package "mongoose" use with mongodb for build schema
 
```

### 2. start MongoDB
```
 mongod --dbpath ./data
 sudo apt-get install libkrb5-dev   ---> สำหรับ ubuntu ต้องลง 
```
