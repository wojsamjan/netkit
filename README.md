# netkit
Installation and setting up

1. According to [FAQ - Netkit Wiki](http://wiki.netkit.org/index.php/FAQ#On_every_attempt_to_start_a_virtual_machine_I_get_the_error:_.22Can.27t_execvp_some_path.2Fkernel.2Fnetkit-kernel:_No_such_file_or_directory.22._But_the_kernel_file_is_there.21_What_is_going_wrong.3F) install 32-bit compatibility libraries:

```
sudo apt-get install libc6:i386 libncurses5:i386 libreadline6:i386
```