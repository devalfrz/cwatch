cwatch
======

Linux compass watch automation


Install
======
```
git clone git://github.com/devalfrz/cwatch.git
chmod +x cwatch/cwatch
```
as su:
```
mv cwatch /etc/cwatch
ln -s /etc/cwatch/cwatch /etc/init.d/cwatch
sudo update-rc.d cwatch defaults
```
Usage
======

as su:
```
/etc/init.d/cwatch start   # Start watching projects on the dirs.conf
/etc/init.d/cwatch stop  # Stops all compass watched projects
/etc/init.d/cwatch restart  # Stops all compass watched projects and starts watching projects on the dirs.conf
```

Uninstall
======
To avoid the proccess from starting at boot just run as su:
```
sudo update-rc.d -f cwatch remove
```
