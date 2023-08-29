## Build DPDK
1、Downlaod dpdk

22.11 is prefered

2、Compile DPDK
```
meson -Dmachine=x86-64-v2 -Ddisable_libs="" build
```
`machine`: we choose march=x86-64-v2 for better portbility between Intel & AMD CPUs

`disable_libs` : we enable kni lib in DPDK buikld, by default DPDK 22.11 disable the kni and other libs when building

## Runtime Require
libatomic

libbsd
