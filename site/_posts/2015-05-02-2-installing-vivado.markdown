---
layout: post
title:  "Installing Vivado on Ubuntu 14.04"
date:   2015-05-02 12:00:00
categories: jekyll update
excerpt: Vivado is software from Xilinx that will enable us to program Zynq devices. This note shows how to install Vivado on Ubuntu. 
screenshot: note-2.jpg
note: 2
---

We just [installed Ubuntu on VMware in MAC]({{site.baseurl}}/1-installing-ubuntu). Now we're going to install Vivado so we can play with the Xilix Zynq device. 

For reference you can look at Vivado install notes: [UG973 (v2015.1) April 1, 2015](http://www.xilinx.com/support/documentation/sw_manuals/xilinx2015_1/ug973-vivado-release-notes-install-license.pdf)

To start, open a terminal and run the following commands.

{% highlight bash %}
cd Downloads/
chmod 777 Xilinx_Vivado_SDK_2015.1_0428_1_Lin64.bin
sudo ./Xilinx_Vivado_SDK_2015.1_0428_1_Lin64.bin
{% endhighlight %}

![Run these commands]({{ site.baseurl }}/assets/note-2/install-vivado-1.png)

The Vivado GUI will show up. Click next to continue.

![Click Next]({{ site.baseurl }}/assets/note-2/install-vivado-2.png)

We are going to use the free WebPACK license. Select that and click next.

![Select WebPACK and click next]({{ site.baseurl }}/assets/note-2/install-vivado-3.png)

We don't need the 7 series devices, just the Zynq. If you're going to use any 7 Series devices make sure to select them on this page. 

![Select WebPACK and click next]({{ site.baseurl }}/assets/note-2/install-vivado-4.png)

We will let the installer choose the default location and click 'Yes' to let it create `/opt/Xilinx` directory. 

![Select WebPACK and click next]({{ site.baseurl }}/assets/note-2/install-vivado-5.png)

Looks good, click next to download and install. 

![Select WebPACK and click next]({{ site.baseurl }}/assets/note-2/install-vivado-6.png)

We're done! Check the next post about running Vivado and creating a project.

[Previous Note]({{site.baseurl}}/1-installing-ubuntu) - [Next Note]({{site.baseurl}}/3-running-vivado)

