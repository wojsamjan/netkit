# netkit
Installation and setting up netkit on a 64-bit linux machine

1. According to [FAQ - Netkit Wiki](http://wiki.netkit.org/index.php/FAQ#On_every_attempt_to_start_a_virtual_machine_I_get_the_error:_.22Can.27t_execvp_some_path.2Fkernel.2Fnetkit-kernel:_No_such_file_or_directory.22._But_the_kernel_file_is_there.21_What_is_going_wrong.3F) install 32-bit compatibility libraries:

```
sudo apt-get install libc6:i386 libncurses5:i386 libreadline6:i386
```

2. Download: ```the Netkit "core", the Netkit filesystem, the Netkit kernel``` [Latest Stable Release](http://wiki.netkit.org/index.php/Download_Official#Latest_Stable_Release)

3. Then unpack them by using the following commands:

```
tar -xjSf netkit-x.y.tar.bz2
tar -xjSf netkit-filesystem-Fx.y.tar.bz2
tar -xjSf netkit-kernel-Kx.y.tar.bz2
```

Note: all the three packages must be uncompressed while staying in the same directory.
