# About This Project
nVidia CUDA drivers are provided for Ubuntu only. Sadly they will depend on a `screen-resolution-extra` package. This seems to be nothing more but a couple of scripts to provide UI widget for fast screen resolution change. As this package is not available for Debian, `nvidia-driver` does not install.

This project builds a stub package `screen-resolutioon-extra-nogui` to satisfy driver package dependencies. It does not provide any functionality, however.

# Installation
Please visit http://pkg.baltnet.net for instructions how to configure Baltnet repository and install this package.

# Configuration
There is no default working configuration which a daemon can use. Therefore, a custom configuration must be created manually after installation.
