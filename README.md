# baremetal
A baremetal greenfield install script for IOST development environment.  Currently supports Ubuntu 16.04, 16.10, 18.04 and 18.10.

Please read carefully as these are hard requirements:

  1.  This is for a greenfield install, do not install on a configured system.
  2.  Do not run as the root user.  Run under a user that can sudo to root (man visudo).
  3.  This is ALPHA level software and there are no official releases, use at your own risk.

This script will install the following:

  -  Security updates and patches for Ubuntu 
  -  Rocks DB v5.14.3
  -  Golang verson 1.11.3
  -  nvm version v0.33.11
  -  node version v10.14.2
  -  npm version v6.4.1
  -  docker version v18.06.0-ce
  -  nvm version v0.33.11
  -  Dependencies; software-properties-common, build-essential, curl, git, git-lfs, and more

IOST
  -  Currently pulls from github.com/iost-official/go-iost
  -  Will build iWallet, iServer, and the dApp deve environment
  -  See official dev docs at https://developers.iost.io
  -  Keep up with IOST developer news:  https://iost.news


# installation
```
git clone https://github.com/iost-unofficial/baremetal.git
cd baremetal
./bootstrap.sh
```

