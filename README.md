
binary --- prebuild deb package under ubuntu 14.04 
source --- source code of openni2 which support percipio depth sensor


Build package

------------------------------------------------
cd source
dpkg-source -x openni2_2.2.0.33+dfsg-4.dsc
cd openni2-2.2.0.33+dfsg
dpkg-buildpackage -j1

------------------------------------------------
Note: make sure to use '-j1' when building in ARM platform



Install Package

------------------------------------------------

dpkg -i libopenni2-0_2.2.0.33+dfsg-4_amd64.deb
dpkg -i libopenni2-dev_2.2.0.33+dfsg-4_amd64.deb

------------------------------------------------
