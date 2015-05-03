---
layout: post
title:  "Adding board definition files to Vivado"
date:   2015-05-02 12:00:00
categories: jekyll update
excerpt: To create Vivado designs for specific boards, board definition files can be used. This note shows how to install the board defintion files for Avnet PicoZed boards.
screenshot: note-4.jpg
note: 4
---

The board we're going to use is the [PicoZed 7030](http://zedboard.org/product/picozed), the board files are not included in Vivado by default so we need to add them. 

For the Picozed, there are several places to look for documentation. 

[PicoZed carrier board](http://zedboard.org/support/documentation/4701)
[PicoZed board](http://zedboard.org/support/documentation/4736)

The board definition files are located in the [PicoZed carrier board](http://zedboard.org/support/documentation/4701) documentation. Navigate there and download the 'Board Definition Files'.

![Download board definition files]({{ site.baseurl }}/assets/note-4/install-bdf-1.png)

Unzip and copy the files from boards, the commands I used are below.

{% highlight bash %}
cd ~/Downloads/
unzip Install\ Avnet\ Board\ Definition\ Files\ in\ Vivado\ 2014.x\ v1.5.zip 
unzip Avnet\ PicoZed\ Boards\ 2014_x_150224.zip
cd boards/board_parts/zynq
cp * /opt/Xilinx/Vivado/2015.1/data/boards/board_parts/zynq/
{% endhighlight %}

The board files should be visible in the `/opt/Xilinx/Vivado/2015.1/data/boards/board_parts/zynq/` folder.

![Download board definition files]({{ site.baseurl }}/assets/note-4/install-bdf-2.png)

Now we're ready to make the first Vivado project! 

[Previous Note]({% post_url 2015-05-02-3-running-vivado %}) - [Next Note]({% post_url 2015-05-02-5-creating-a-project %})