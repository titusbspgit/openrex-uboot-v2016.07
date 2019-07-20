# openrex_uboot_v2016_07
mx6q/dl/s/spl openrex u-boot v2016.07
 
# Download repository
    git clone https://github.com/titusbspgit/openrex-uboot-v2016.07.git
    cd openrex-uboot-v2016.07
 
# Install cross compiler
    apt-get install gcc-arm-linux-gnueabihf
 
# Setup cross compiler
    export CROSS_COMPILE=arm-linux-gnueabihf-
    export ARCH=arm
 
# Build (imx6q)
    make distclean
    make mx6qopenrex_config
    make
    cp u-boot.imx /tftp/uboot-mx6qopenrex.imx
 
# Build (imx6dl)
    TODO
 
# Build (imx6s)
    TODO
