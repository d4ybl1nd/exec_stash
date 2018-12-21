
Current build of CentOS uses 2.33 of util-linux. [:Bug Tracker](https://bugs.centos.org/view.php?id=15170)

There's way to install util-linux 2.29 <= [:Build Service](https://cbs.centos.org/koji/packageinfo?packageID=146)

[-> rpm info](https://cbs.centos.org/koji/rpminfo?rpmID=81561)

[-> Build info](https://cbs.centos.org/koji/buildinfo?buildID=15169)

some of basic unix tools were missing a lots of options

Going to add a script to sort this out. 

So, here is the list.

## Dependencies
 - /bin/sh <br/>
 - /etc/pam.d/system-auth <br/>
 - audit-libs >= 1.0.6 <br/>
 - config(util-linux) = 2.29-2.el7 <br/>
 - coreutils <br/>
 - ld-linux-x86-64.so.2()(64bit) <br/>
 - ld-linux-x86-64.so.2(GLIBC_2.3)(64bit) <br/>
 - libaudit.so.1()(64bit) <br/>
 - libblkid = 2.29-2.el7 <br/>
 - libblkid.so.1()(64bit) <br/>
 - libblkid.so.1(BLKID_1.0)(64bit) <br/>
 - libblkid.so.1(BLKID_2.15)(64bit) <br/>
 - libblkid.so.1(BLKID_2.17)(64bit) <br/>
 - libblkid.so.1(BLKID_2.18)(64bit) <br/>
 - libblkid.so.1(BLKID_2.20)(64bit) <br/>
 - libblkid.so.1(BLKID_2.21)(64bit) <br/>
 - libblkid.so.1(BLKID_2.25)(64bit) <br/>
 - libc.so.6()(64bit) <br/>
 - libc.so.6(GLIBC_2.10)(64bit) <br/>
 - libc.so.6(GLIBC_2.11)(64bit) <br/>
 - libc.so.6(GLIBC_2.12)(64bit) <br/>
 - libc.so.6(GLIBC_2.13)(64bit) <br/>
 - libc.so.6(GLIBC_2.14)(64bit) <br/>
 - libc.so.6(GLIBC_2.15)(64bit) <br/>
 - libc.so.6(GLIBC_2.16)(64bit) <br/>
 - libc.so.6(GLIBC_2.17)(64bit) <br/>
 - libc.so.6(GLIBC_2.2.5)(64bit) <br/>
 - libc.so.6(GLIBC_2.3)(64bit) <br/>
 - libc.so.6(GLIBC_2.3.4)(64bit) <br/>
 - libc.so.6(GLIBC_2.4)(64bit) <br/>
 - libc.so.6(GLIBC_2.6)(64bit) <br/>
 - libc.so.6(GLIBC_2.7)(64bit) <br/>
 - libc.so.6(GLIBC_2.8)(64bit) <br/>
 - libc.so.6(GLIBC_2.9)(64bit) <br/>
 - libcap-ng.so.0()(64bit) <br/>
 - libcrypt.so.1()(64bit) <br/>
 - libcrypt.so.1(GLIBC_2.2.5)(64bit) <br/>
 - libfdisk = 2.29-2.el7 <br/>
 - libfdisk.so.1()(64bit) <br/>
 - libfdisk.so.1(FDISK_2.26)(64bit) <br/>
 - libfdisk.so.1(FDISK_2.27)(64bit) <br/>
 - libfdisk.so.1(FDISK_2.28)(64bit) <br/>
 - libfdisk.so.1(FDISK_2.29)(64bit) <br/>
 - libm.so.6()(64bit) <br/>
 - libmount = 2.29-2.el7 <br/>
 - libmount.so.1()(64bit) <br/>
 - libmount.so.1(MOUNT_2.19)(64bit) <br/>
 - libmount.so.1(MOUNT_2.20)(64bit) <br/>
 - libmount.so.1(MOUNT_2.21)(64bit) <br/>
 - libmount.so.1(MOUNT_2.22)(64bit) <br/>
 - libmount.so.1(MOUNT_2.23)(64bit) <br/>
 - libmount.so.1(MOUNT_2.24)(64bit) <br/>
 - libmount.so.1(MOUNT_2.25)(64bit) <br/>
 - libncursesw.so.5()(64bit) <br/>
 - libpam.so.0()(64bit) <br/>
 - libpam.so.0(LIBPAM_1.0)(64bit) <br/>
 - libpam_misc.so.0()(64bit) <br/>
 - libpam_misc.so.0(LIBPAM_MISC_1.0)(64bit) <br/>
 - librt.so.1()(64bit) <br/>
 - librt.so.1(GLIBC_2.2.5)(64bit) <br/>
 - librt.so.1(GLIBC_2.3.3)(64bit) <br/>
 - libselinux.so.1()(64bit) <br/>
 - libsmartcols = 2.29-2.el7 <br/>
 - libsmartcols.so.1()(64bit) <br/>
 - libsmartcols.so.1(SMARTCOLS_2.25)(64bit) <br/>
 - libsmartcols.so.1(SMARTCOLS_2.27)(64bit) <br/>
 - libsmartcols.so.1(SMARTCOLS_2.28)(64bit) <br/>
 - libsystemd.so.0()(64bit) <br/>
 - libsystemd.so.0(LIBSYSTEMD_209)(64bit) <br/>
 - libtinfo.so.5()(64bit) <br/>
 - libudev.so.1()(64bit) <br/>
 - libudev.so.1(LIBUDEV_183)(64bit) <br/>
 - libutempter.so.0()(64bit) <br/>
 - libutempter.so.0(UTEMPTER_1.1)(64bit) <br/>
 - libutil.so.1()(64bit) <br/>
 - libutil.so.1(GLIBC_2.2.5)(64bit) <br/>
 - libuuid = 2.29-2.el7 <br/>
 - libuuid.so.1()(64bit) <br/>
 - libuuid.so.1(UUID_1.0)(64bit) <br/>
 - libz.so.1()(64bit) <br/>
 - pam >= 1.1.3-7 <br/>
 - rpmlib(CompressedFileNames) <= 3.0.4-1 <br/>
 - rpmlib(FileDigests) <= 4.6.0-1 <br/>
 - rpmlib(PayloadFilesHavePrefix) <= 4.0-1 <br/>
 - rpmlib(PayloadIsXz) <= 5.2-1 <br/>
 - rtld(GNU_HASH) <br/>
