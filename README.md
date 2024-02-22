# xrdp-modern-login

## Overview
After you have performed an xRDP installation, you should see the standard 
and slightly dated xRDP login screen.  The idea is to modernize the xRDP 
login screen a little, using the configuration (colors and positions) and
combining it with the possibility of adding a custom image.

## Quick Start

The XRDP customization possibilities are limited.  To change the look’n feel
of the xRDP login screen, you need to edit the file `/etc/xrdp/xrdp.ini`.  
The colors we use are quite basic and minimalist, always keep in mind that 
you can modify them to your liking. This customization gives you an idea of
how to do something new.

This is what the customization looks like once finished:

![demo](https://github.com/dAvidcA/xrdp-modern-login/assets/585236/ccc72055-50dd-4e44-90ff-967a0e7f3db8)

**Note:** The image shared in the repository (`/usr/share/xrdp/xrdp-logo.bmp`) 
does not have the avatar and logo name of my server (danbo), it is an image
that you can edit (with the image editor of your choice), customize and add
the details to your liking.

### Example custom design

![example](https://github.com/dAvidcA/xrdp-modern-login/assets/585236/a314364f-b3ff-4f08-96c0-229e37e9bda7)


## How to use

  * It is recommended to backup the old *xrdp.ini* file which is stored
    under `/etc/xrdp/xrdp.ini` (Just in case you need it later)
  * Copy the new *xrdp.ini* on `/etc/xrdp/`
  * Copy the new logo *xrdp-logo.bmp* on `/usr/share/xrdp/`. Remember
    to edit the image and add your fav design. The image must be in 24-bits
    bitmap (.bmp)
  * Reboot your server or restart the xRDP service: `sudo service xrdp restart`
