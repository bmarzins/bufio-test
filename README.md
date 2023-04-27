# Requirements

All the tools necesary to build the kernel and a built kernel with the
configuration and header files. For packaged kernels,  these will be in the
kernel-devel or kernel-headers packages.

# Building the module for the running kernel

    make -C /lib/modules/`uname -r`/build M=$PWD

# Installing the module

    make -C /lib/modules/`uname -r`/build M=$PWD modules_install
