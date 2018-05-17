C.R.A.SSH-docker
=========

C.R.A.SSH (*crassh*) stands for *Cisco Remote Automation via SSH*, it is
a python script for automating commands on Cisco devices.

[![Travis CI: continuous integration status](https://travis-ci.org/linickx/crassh.svg?branch=master)](https://travis-ci.org/linickx/crassh)
[![Documentation Status](https://readthedocs.org/projects/crassh/badge/?version=latest)](http://crassh.readthedocs.org/en/latest/?badge=latest)

Crassh can be used in two ways:

-   a stand alone script that users (*Network Admins*) can run to
    perform actions on Cisco devices
-   a module developers can import and leverage in their own scripts

The **documentation is available here:** <http://crassh.readthedocs.org>

The author's [personal blog](http://www.linickx.com) contains a [tutorial
here](http://www.linickx.com/3980/automating-cisco-commands-with-c-r-a-ssh)
on how to use crassh in standalone mode and an [initial
example](http://linickx.com/pip-install-crassh) on how to use the crassh
module. Future [news about crassh can be found
here](http://www.linickx.com/tag/crassh).


## Example


```bash
$ docker run -it bernadinm/crassh python crassh.py
```

```bash
$ docker run -v $PWD:$PWD -it bernadinm/crassh python crassh.py -s $PWD/switch -c $PWD/commands -U username -P password
```



Disclaimer
----------

The word *Cisco* is used as a description because this script should
work with any Cisco IOS device. Cisco is a registered trademark of Cisco
Systems Inc; this script is not associated, endorsed, supported or
affiliated in any way with Cisco and none of these are implied.

