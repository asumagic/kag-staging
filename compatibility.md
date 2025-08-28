# Important compatibility information

## 64-bit requirement

You now need a 64-bit operating system to run KAG (both on Linux and on Windows). Very few people use 32-bit operating systems nowadays, but it is worth mentioning.  
This comes with simpler tooling support for us, improved compatibility and enhances performance.

This means that on Linux you do not need to install 32-bit compatibility libraries in order to run the standalone game or a dedicated server.

## Linux glibc requirements

KAG is now built to target Ubuntu 22.04. We attempt to keep ABI compatibility with older glibc (down to 2.17, from 2012), but please understand that this is retrocompatibility is best-effort only and there are reasons why we can't always ship certain updated libraries such as the libstdc++.
If you are running on an older Linux distribution that ships an outdated glibc or libstdc++ version, you may need to upgrade.
