## About
We have received numerous requests about bringing support for Ubuntu 20.04 LTS sooner. This repo will be the home for testers, before official support will be delivered by us.

## Installation
All you need to do to start with Webmin on Ubuntu 20.04 LTS is to install custom "python" package that only contains a symlink to `/usr/bin/python3` binary. To start with Virtualmin, you would need to install all other "dummy" packages listed in this repo, and run slightly modified install script.

## Post-Installation
At the moment, Webmin 1.941 is installed by default, which doesn't contain important fixes for Ubuntu _netplan_, bringing better support - you would need to install it manually from [devel repo](https://download.webmin.com/devel/deb/). For Virtualmin, you would need to apply latest MariaDB patches [@c8a8596](https://github.com/virtualmin/virtualmin-gpl/commit/c8a8596f05342873d05de29b55ded688fef5480f), [@20faaa7](https://github.com/virtualmin/virtualmin-gpl/commit/20faaa725478109898b2d13517a56c82288e55a1), which you can do easily by replacing [feature-mysql.pl](https://github.com/virtualmin/virtualmin-gpl/blob/master/feature-mysql.pl) file, so you'd be able to set db user password at Virtualmin post-installation wizard.

## Screenshots
![](https://github.com/iliarostovtsev/webmin-virtualmin-ubuntu20-dev/blob/master/screenshots/vm-u20-post-install.png)
![](https://github.com/iliarostovtsev/webmin-virtualmin-ubuntu20-dev/blob/master/screenshots/vm-u20-config-check.png)

## License
Released under the [MIT License](https://github.com/iliarostovtsev/webmin-virtualmin-ubuntu20-dev/blob/master/LICENSE).
