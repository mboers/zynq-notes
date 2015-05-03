---
layout: post
title:  "Creating a Vivado project"
date:   2015-05-02 12:00:00
categories: jekyll update
excerpt: Getting started with Zynq on Windows. We will install Vivado 2014.4 and create the first project.
screenshot: note-5.png
note: 5
---

In this note we'll create a Vivado project and make an LED flash. 

Open Vivado and select __Create New Project__.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-1.png)

Click __Next__.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-2.png)

Enter a project name, then click __Next__.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-3.png)

Choose __RTL project__, then click __Next__.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-4.png)

Click __Next__, we'll add sources later. 

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-5.png)

Click __Next__, we don't need to add any IP. 

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-6.png)

Click __Next__, no constraints needed yet. 

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-7.png)

Click __Boards__ and choose __PicoZed 7030 SOM + Carrier__, this is one of the boards we added in the previous note. 

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-8.png)

Finally, check everything is OK and click __Finish__. 

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-9.png)

We're now presented with the workspace. Click __create block design__ in the left hand navigator to add a new block to the project.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-10.png)

A dialog will pop-up, choose a block design name and click __OK__.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-11.png)

In the top right of the application, a black block design will open. Right click on this and click __Add IP__.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-12.png)

Type _zynq_ and when __ZYNQ7 Processing System__ is highlighted hit __Enter__. This will place the Zynq hardware macro into the design.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-13.png)

Click __Run Block Automation__ link in the banner at the top of the design canvas. [UG994](http://www.xilinx.com/support/documentation/sw_manuals/xilinx2015_1/ug994-vivado-ip-subsystems.pdf) describes block automation in more detail: 

> IP integrator offers a feature called Designer Assistance, which includes Block Automation
and Connection Automation, to assist you in putting together a basic microprocessor
system by making internal connections between different blocks and making connections
to external interfaces. The Block Automation Feature is provided when an embedded
processor such as the Zynq® Processing System 7 or MicroBlaze™ processor, or some other
hierarchical IP such as an Ethernet is instantiated in the IP integrator block design. 

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-14.png)

The __Run Block Automation__ dialog opens, no need to change anything, click __OK__.

![Create a new project]({{ site.baseurl }}/assets/note-5/create-vivado-15.png)

[Previous Note]({{site.baseurl}}/4-adding-board-files) - Coming Soon

