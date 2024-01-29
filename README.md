# Synergy Binaries
Synergy is a tool that lets you use the same mouse & keyboard across Windows, Mac and Linux. Here you can find the latest freely available Synergy binaries (before Synergy went closed source). Synergy no longer openly distribute binaries, to get the latest version of Synergy you must pay for it. If you want to learn more about Synergy or get the paid version [click here](https://symless.com/synergy).

## Latest release candidate (v1.9.0-rc3)
This version fixes a few macOS bugs found in v1.8.8 and has an updated GUI. Binaries were found [here](https://members.symless.com/forums/topic/2587-download-synergy-19-rc3-fixes-the-macos-wifi-lag-bug/).

* Windows 7 and later 64-bit: [Synergy_v1.9.0_rc3.msi](https://github.com/amankhoza/synergy-binaries/raw/master/Synergy_v1.9.0_rc3.msi)
* macOS 10.9 and later 64-bit: [Synergy_v1.9.0_rc3.dmg](https://github.com/amankhoza/synergy-binaries/raw/master/Synergy_v1.9.0_rc3.dmg)
* CentOS/Fedora 64-bit: [Synergy-1.9.0_rc3-1.x86_64.rpm](https://github.com/amankhoza/synergy-binaries/raw/master/Synergy-1.9.0_rc3-1.x86_64.rpm)
* Debian 8 (Jessie) 64-bit: [Synergy_1.9.0~rc3_amd64_debian.deb](https://github.com/amankhoza/synergy-binaries/raw/master/Synergy_1.9.0~rc3_amd64_debian.deb)
* Ubuntu LTS (16.04 LTS or later) 64-bit: [Synergy_1.9.0~rc3_amd64_ubuntu.deb](https://github.com/amankhoza/synergy-binaries/raw/master/Synergy_1.9.0~rc3_amd64_ubuntu.deb) [[see here]](https://github.com/amankhoza/synergy-binaries/edit/master/README.md#required-dependencies-for-synergy-v190-rc3-on-ubuntu)

## Latest stable release (v1.8.8-stable)
This is the last released stable version of Synergy. Binaries were found [here](https://github.com/brahma-dev/synergy-stable-builds/releases).

* Windows 32-bit: [synergy-v1.8.8-stable-Windows-x86.msi](https://github.com/amankhoza/synergy-binaries/raw/master/synergy-v1.8.8-stable-Windows-x86.msi)
* Windows 64-bit: [synergy-v1.8.8-stable-Windows-x64.msi](https://github.com/amankhoza/synergy-binaries/raw/master/synergy-v1.8.8-stable-Windows-x64.msi)
* Mac OSX 64-bit: [synergy-v1.8.8-stable-MacOSX-x86_64.dmg](https://github.com/amankhoza/synergy-binaries/raw/master/synergy-v1.8.8-stable-MacOSX-x86_64.dmg)
* CentOS/Fedora 32-bit: [synergy-v1.8.8-stable-Linux-i686.rpm](https://github.com/amankhoza/synergy-binaries/raw/master/synergy-v1.8.8-stable-Linux-i686.rpm)
* CentOS/Fedora 64-bit: [synergy-v1.8.8-stable-Linux-x86_64.rpm](https://github.com/amankhoza/synergy-binaries/raw/master/synergy-v1.8.8-stable-Linux-x86_64.rpm)
* Ubuntu/Debian 32-bit: [synergy-v1.8.8-stable-Linux-i686.deb](https://github.com/amankhoza/synergy-binaries/raw/master/synergy-v1.8.8-stable-Linux-i686.deb)
* Ubuntu/Debian 64-bit: [synergy-v1.8.8-stable-Linux-x86_64.deb](https://github.com/amankhoza/synergy-binaries/raw/master/synergy-v1.8.8-stable-Linux-x86_64.deb)

## Older releases
Older releases and source code can be found [here](https://github.com/brahma-dev/synergy-stable-builds/releases).

## Required dependencies for Synergy v1.9.0-rc3 on Ubuntu
```
#Downloading libssl1.0.0 package from official Ubuntu repository
wget http://security.ubuntu.com/ubuntu/pool/main/o/openssl1.0/libssl1.0.0_1.0.2n-1ubuntu5.10_amd64.deb
#Installing libssl1.0.0 package
sudo dpkg -i libssl1.0.0_1.0.2n-1ubuntu5.10_amd64.deb
#Adding PPA repository for package that allows use of libcurl3 and libcurl4 at the same time
sudo add-apt-repository ppa:xapienz/curl34
#Updating apt cache
sudo apt update
#Installing libcurl3 and libcurl4 package
sudo apt install libcurl4=7.68.0-1ubuntu2.5ppa1
#Installing dependencies required by Synergy
sudo apt install libavahi-compat-libdnssd1 qml-module-qtquick-controls qml-module-qtquick-layouts qml-module-qtquick-dialogs qml-module-qtquick2 qml-module-qtgraphicaleffects qml-module-qtquick-window2 qml-module-qtquick-privatewidgets
```
