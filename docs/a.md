# Verifying the CPU

I can support Windows 10/11 or any edition of Windows Server 2016 or better. My practical exercises have not been tested on MAC OS and will probably not work on Apple hardware since the change to Mx processors.

There are some specific requirements before you can use your Windows 10/11 computer as a virtualization platform. The first thing we need to do is to understand what hardware is in the computer. We can verify most of what we need using __systeminfo.exe__ from the command prompt.

In the example below, I’m running a Windows 11 Education instance.

<figure>
<img src = "https://jor-donegal.github.io/verify26/images/fig1.jpg">
<figcaption>Fig 1. SYSINFO on a VMWare PC.</figcaption>
</figure>

Note that it tells me a hypervisor has been detected. This machine has VMWare Workstation installed.

Contrast that to one of my older Windows 10 machines, which has Hyper-V installed.

<figure>
<img src = "https://jor-donegal.github.io/verify26/images/fig2.jpg">
<figcaption>Fig 2. SYSINFO on a Huper-V PC.</figcaption>
</figure>


In the previous screenshots I can see exactly the type of processor I have, the motherboard, and how much RAM I am using. At the end of this screenshot I can see the status of critical properties for virtualization. And they are all good! There are other things I can see that are mandatory for virtualization;

- A 64-bit version of Windows.
- The professional or education version.
- Enough main memory (32GB).
