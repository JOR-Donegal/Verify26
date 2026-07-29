# Secondary Storage

I also need to map the available disks and see if I have suitable secondary storage for virtual machines. If I run __diskpart.exe__ and then type the command __list disk__, I can get an idea of what disks are in my system.

<figure>
<img src = "https://jor-donegal.github.io/Verify26/images/fig3.avif">
<figcaption>Fig 3. List disk.</figcaption>
</figure>

I need to determine which disks are _spinning disks_ (HDD) and which are _solid-state_ (SSD). A quick way to do this is to run __dfrgui.exe__, the _defragmentation_ tool. I can clearly see the drive types in my system.

<figure>
<img src = "https://jor-donegal.github.io/Verify26/images/fig4.avif">
<figcaption>Fig 4. Output from dfrgui.</figcaption>
</figure>

This configuration is actually pretty good;

- C:\ is a small SSD specifically intended for the host operating system.
- I have a dedicated disk E:\ for synchronizing my cloud shares
- A separate dedicated disk F:\ for holding static information, like ISO files.
- Finally, I have a dedicated SSD G:\ for VM’s.

If I was running a lot of VM’s, I could improve the performance by adding more, small SSD’s.