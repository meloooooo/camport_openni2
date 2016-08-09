
1. Install Package

Linux 
 
$dpkg -i libopenni2-0_2.2.0.33+dfsg-4_amd64.deb
$dpkg -i libopenni2-dev_2.2.0.33+dfsg-4_amd64.deb

ARM

$dpkg -i libopenni2-0_2.2.0.33+dfsg-4_armhf.deb
$dpkg -i libopenni2-dev_2.2.0.33+dfsg-4_armhf.deb


2. Build package (Optional)

------------------------------------------------
cd source
dpkg-source -x openni2_2.2.0.33+dfsg-4.dsc
cd openni2-2.2.0.33+dfsg
dpkg-buildpackage -j1

------------------------------------------------
Note: 
a. make sure to use '-j1' when building in ARM platform
b. if you failed to open the camera device with permission reason,
copy the usb rules 
   $sudo cp binary/primesense-usb.rules /etc/udev/rules.d/
