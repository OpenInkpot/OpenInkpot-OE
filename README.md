OpenInkpot-OE
=============
git submodule init

git submodule update --remote

source poky/oe-init-build-env build

cp ../conf/bblayers.conf ../conf/local.conf conf/

DISTRO=openinkpot MACHINE=eb600 bitbake core-image-oi-dev
