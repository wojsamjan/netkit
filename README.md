# netkit
Installation and setting up netkit on a 64-bit linux machine

1. According to [FAQ - Netkit Wiki](http://wiki.netkit.org/index.php/FAQ#On_every_attempt_to_start_a_virtual_machine_I_get_the_error:_.22Can.27t_execvp_some_path.2Fkernel.2Fnetkit-kernel:_No_such_file_or_directory.22._But_the_kernel_file_is_there.21_What_is_going_wrong.3F) install 32-bit compatibility libraries:

```
sudo apt-get install libc6:i386 libncurses5:i386 libreadline6:i386
```

2. Download: ```the Netkit "core", the Netkit filesystem, the Netkit kernel``` [Latest Stable Release](http://wiki.netkit.org/index.php/Download_Official#Latest_Stable_Release).

3. Then unpack them by using the following commands:

```
tar -xjSf netkit-x.y.tar.bz2
tar -xjSf netkit-filesystem-Fx.y.tar.bz2
tar -xjSf netkit-kernel-Kx.y.tar.bz2
```
+ Note: All the three packages must be uncompressed while staying in the same directory.
+ Note: Once Netkit has been unpacked, no root privileges are required to configure it and start working.

4. Set the environment variable NETKIT_HOME to the name of the directory Netkit has been installed into. Assuming that you have installed Netkit to /home/yashimoto/Pulpit/netkit/netkit and that your shell is bash, you would use the following commands:
```
export NETKIT_HOME=/home/yashimoto/Pulpit/netkit/netkit
export MANPATH=:$NETKIT_HOME/man
```
+ Note: It may also be useful to put these lines inside ```'.bashrc' located mostly in your /home or /etc directory```.

5. Update your PATH environment variable to include the path to the standard Netkit commands. Assuming Netkit is (still) installed into /home/yashimoto/Pulpit/netkit/netkit and that your shell is (still) bash, you would type:
```
export PATH=$NETKIT_HOME/bin:$PATH
```
+ Note: Again, put this line inside ```'.bashrc'```.
