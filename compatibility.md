# Important compatibility information

## 64-bit support

You now need a 64-bit operating system to run KAG. This is almost always the case already, but it is worth mentioning.

This comes with simpler tooling support for us and enhances performance.

## Bumped minimal Linux requirement

KAG is now built to target Ubuntu 18.04.  
This should not cause issues, but you may need to upgrade to a newer version if you are running on an ancient Linux distribution that ships a libc or libstdc++ version that we do not support.

## Dropped macOS support

Due to the lack of developer resources to port the new version to macOS and due to being a hostile development platform for developers who do not own Apple hardware, macOS support has been dropped completely for now.

Since the Windows build is now 64-bit, however, you should be able to run KAG unofficially using `wine64`, which is compatible with macOS Catalina (which dropped 32-bit support that KAG used to rely on).