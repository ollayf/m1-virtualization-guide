# Guide to Virtualization on Apple Silicon
As the M1 ecosystem is being built up, there are many reasons to want to utilise other OS's for your Mac. At the time of this writing, there are a few main ways to accomplish this, broadly speaking:
1. Virtualization
2. Emulation
3. Dual Booting

As much as possible I will try to experiment with the aforementioned technologies, and different software that can be used to achieve them.  

If you are interested to help out, or have used any of the following that I have not tested, feel free to [holler](#Contact). 

## Note: 
As much as possible, I will try to focus more on function rather than simplicity. Some of these will require you to go into config files/ BIOS/ terminal. As long as you follow the guides and understand what is going on, you will be fine.

# Foreword
As an engineering/ computing student, you must have had seniors dissuading you from using the m1 macbook given its current instability. The fact that you still chose this path is definitely commendable, however, the inescapable fact is that a lot of software may not be native/ simple to install. This repository was created in order to aide you in your journey. Please consider contributing if you are part of the m1 gang gang so that you may help others as well.  

# Disclaimer
I do not take any responsibility for any crashes, failures as a result of following this guide. Use this at your own discretion. These guides/ documentations are supposed to work at the time of its writing, but may not at the time you are using it. If you have any issues, feel free to submit it and hopefully someone will support you.

# ARM architecture
This is a fascinating technology, which also remains one of the biggest reasons for me to make this purchase. If you haven't heard of this term (or RISC-V), I shall spare you the details, however, the main point is that the architecture of the macbook is very similar to that of a raspberry pi. Hence, I will be mostly using that as a reference for software that are generally more stable.

## [Best Linux Distros for arm64](https://www.maketecheasier.com/best-linux-distributions-for-arm-devices/)

1. Debian
2. Ubuntu 
2. ArchLinux
3. Manjaro
4. Chromium

Personally, I have tried and used ubuntu on arm64 and it was a very good experience. If you are a very new user of linux to the point where you don't at least know the general differences between these, just stick with debian, or ubuntu. It's really simple due to everything more or less being packaged nicely for you. **apt** is really sweet as well!

## [Vivado Design **NOT SUPPORTED**](https://forums.xilinx.com/t5/Installation-and-Licensing/Vivado-on-ARM-Linux/m-p/1201451)
As of now, Vivado design, as well as many Xilinx tools are not supported by arm64 architecture. RIP Com Eng students

# VMs
Likely the option with the greatest overhead. However, also usually the simplest to set up. You will definitely need to learn how to use VMs eventually tho...   Typically, virtualization can only be done with the same architecture, (at least RISC-V VS CISC-V), but in this case UTM can spin up VMs in different architecture. Greater explanation in the [notes](#notes)

At the time of this writing, there are only a few options available for use on the m1:
1. Parallels Desktop (no intentions of testing)
2. VMWare Fusion 12
3. Virtual Box 6.1
4. **UTM (free)** 
5. ACVM 

## Note
ACVM and UTM are technically emulation software as they use the QEMU engine in the backend. However, it is primarily used to spin up VMs. It is to be noted

# Docker
Containerisation. This is a technology rising in popularity-- lightweight, less resource intensive. Docker strives to run a minimalistic, light containers that are sufficient for whatever app you are using. Consider this.
- [Vivado Design Suite](http://phwl.org/2020/xilinx-vivado-on-ubuntu-using-docker/)

# Emulation
This is basically a smaller, less resource intensive virtualization than a whole VM.
1. CodeWeavers CrossOver (based on Wine)
2. QEMU
3. Wine 5

# Dual Booting
Least overhead, but less stable.
1. Boot Camp (Windows only)
2. Manual

Based on what I understand about Boot Camp, it only allows for use with Windows OS (disgusting), but **DOES NOT** work with **Apple Silicon**.

# Contact
- [Telegram](https://t.me/ollayf)
- [Github](https://github.com/ollayf)