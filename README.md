# Guide to Virtualization on Apple Silicon
As the M1 ecosystem is being built up, there are many reasons to want to utilise other OS's for your Mac. At the time of this writing, there are a few main ways to accomplish this, broadly speaking:
1. Virtualization
2. Emulation
3. Dual Booting

As much as possible I will try to experiment with the aforementioned technologies, and different software that can be used to achieve them.  

## Note: 
As much as possible, I will try to focus more on function rather than simplicity. Some of these will require you to go into config files/ BIOS/ terminal. As long as you follow the guides and understand what is going on, you will be fine.

# Foreword
As an engineering/ computing student, you must have had seniors dissuading you from using the m1 macbook given its current instability. The fact that you still chose this path is definitely commendable, however, the inescapable fact is that a lot of software may not be native/ simple to install. This repository was created in order to aide you in your journey. Please consider contributing if you are part of the m1 gang gang so that you may help others as well.  

# Disclaimer
I do not take any responsibility for any crashes, failures as a result of following this guide. Use this at your own discretion. These guides/ documentations are supposed to work at the time of its writing, but may not at the time you are using it. If you have any issues, feel free to submit it and hopefully someone will support you.

# ARM architecture
This is a fascinating technology, which also remains one of the biggest reasons for me to make this purchase. If you haven't heard of this term (or RISC-V), I shall spare you the details, however, the main point is that the architecture of the macbook is very similar to that of a raspberry pi. Hence, I will be mostly using that as a reference for software that are generally more stable.

# VMs
Easily the option with the greatest overhead. However, also potentially the simplest. You will definitely need to learn how to use VMs eventually tho...  

At the time of this writing, there are only a few options available for use on the m1:
1. Parallels Desktop 
2. UTM

# Docker
Containerisation. This is a technology rising in popularity-- lightweight, less resource intensive. Docker strives to run a minimalistic, light containers that are sufficient for whatever app you are using. Consider this.
- [Vivado Design Suite](http://phwl.org/2020/xilinx-vivado-on-ubuntu-using-docker/)

# Emulation
This is basically a smaller, less resource intensive virtualization than a whole VM.
1. CodeWeavers CrossOver (based on Wine)
2. QEMU
3. Wine (not for m1 macs)

# Dual Booting
Least overhead, but less stable.
1. Boot Camp (Windows only)
2. Manual

Based on what I understand about Boot Camp, it only allows for use with Windows OS (disgusting), but **DOES NOT** work with **Apple Silicon**.

