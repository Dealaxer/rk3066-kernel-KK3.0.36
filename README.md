# rk3066-kernel-KK3.0.36
Kernel for Cube U30GT-H (Android 4.4.4)
<br><br>
<strong>How to compile a kernel for Cube U30GT-H</strong>:<br>
<strong>Install Tools</strong><br>
Command:<br>
<i>apt-get install git-core gnupg flex bison gperf libsdl1.2-dev libesd0-dev libwxgtk3.0-dev build-essential zip curl libncurses5-dev zlib1g-dev lib32z1-dev lib32ncurses5-dev gcc-multilib g++-multilib sharutils lzop</i><br><br>
(To build the kernel 3.0.36 Android 4.4.x, use toolchain with GCC 4.4.3)<br>
Command:<br>
<i>export ARCH=arm</i><br>
<i>export CROSS_COMPILE=(<strong>Your Path</strong>)/toolchain/arm-eabi-4.6/bin/arm-eabi-</i><br><br>

<strong>For Cube U30GT-H should be used RK30 SDK config</strong>:<br>
Command:<br>
<i>make rk30_sdk_defconfig</i>

<strong>Then You can configure kernel with command</strong>:<br>
Command:<br>
<i>make menuconfig</i><br>

<strong>Building the kernel</strong>:<br>
Command:<br>
<i>make -j4</i>

(-j "4" number of threads, that is usually the number of cores of your processor)
