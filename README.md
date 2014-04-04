cwatch
======

Linux compass watch automation


Install
======
git clone git://github.com/devalfrz/cwatch.git
chmod +x cwatch/cwatch
as su:
mv cwatch /etc/cwatch
ln -s /etc/cwatch/cwatch /etc/init.d/cwatch

Usage
======

(as su):
/etc/init.d/cwatch start   # Start watching projects on the dirs.conf
/etc/init.d/cwatch stop  # Stops all compass watched projects
/etc/init.d/cwatch restart  # Stops all compass watched projects and starts watching projects on the dirs.conf
