# About This Project
nVidia CUDA drivers are provided for Ubuntu only. Sadly they will depend on `nvidia-settings` that in turn depends on a `screen-resolution-extra` package. This seems to be nothing more but a couple of scripts to provide UI widget for fast screen resolution change. As this package is not available for Debian, `cuda-drivers` does not install.

This project builds a stub package `screen-resolutioon-extra` to satisfy driver package dependencies. However, it does not provide any functionality.

The best way would actually be to create a virtual package, but [according to Debian policy](https://www.debian.org/doc/debian-policy/#virtual-packages-provides), none of the virtual packages are considered if dependency is defined using a concrete version number. This is exactly, what `nvidia-settings` does. So only solutions would be either to install all the world required by original `screen-resolution-extra` (and this is indeed a Pandora's Box) or use a stub package with a same name as its original counterpart.

# Installation
Please visit http://pkg.baltnet.net for instructions how to configure Baltnet repository and install this package.

# Configuration
There is no default working configuration which a daemon can use. Therefore, a custom configuration must be created manually after installation.
