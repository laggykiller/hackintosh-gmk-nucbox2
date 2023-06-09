# Current status
Tested to work on Monterey, Ventura and Sonoma.

The 3.5mm audio jack does not work, as the device uses ES8336 audio chipset and likely not supported. However, HDMI and USB audio both works.

I do not have the tools to test USB C port display out

I have not thoroughly test it for problems, so please create issue if you find any problem.

I am an amateur in hackintoshing, so I may not be able to help!

Feel free to submit pull requests to help improve this project!

The EFI may work in BeeLink SEi8, but I cannot support it. Please go to https://github.com/daliansky/Beelink-SEI8-Hackintosh

# How to use?
For more details, read dortania guide: https://dortania.github.io/OpenCore-Install-Guide/

You may also take a look at the guide for Intel NUC 8 for reference: https://github.com/zearp/Nucintosh

1. BIOS settings
    - Secure Boot need to be disabled
    - CFG Lock need not be disabled
    - VT-d need not be disabled
2. Create installation USB
3. Download and copy EFI folder to installation USB
4. Edit the following items in config.plist: https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#platforminfo
    - PlatformInfo -> Generic -> MLB
    - PlatformInfo -> Generic -> ROM
    - PlatformInfo -> Generic -> SystemSerialNumber
    - PlatformInfo -> Generic -> SystemUUID
5. Boot the USB and install
6. Copy EFI to hard drive

# Why hackintosh GMK NUCBOX2?
It has very similar spec to Intel NUC 8, which is very hackintosh-able and there are repos for EFI of that device.

However, GMK NUCBOX2 is cheaper than it, making it a good choice for those who want a cheap hackintosh machine.

# Information about GMK NUCBOX2
This is the spec page for the device: https://gmktec.com/products/nucbox2-intel-core-i5-8259u-4k-mini-pc

CPU: Intel Core i5 8279U

GPU: Intel Iris Plus 655

RAM: 2 x 8GB 2666mHz DDR4

Storage: AGI High Performance SSD AI198 M.2 PCIe 1TB

Audio Codec: Intel SST

Ethernet Card: Realtek 8111

Wifi/BT Card: Intel Dual Band Wireless-AC 7265

# Reddit discussion
https://www.reddit.com/r/hackintosh/comments/r9ygp9/gmk_nucbox2_hackintosh/

# Credits
https://dortania.github.io/OpenCore-Install-Guide/

https://github.com/zearp/Nucintosh
