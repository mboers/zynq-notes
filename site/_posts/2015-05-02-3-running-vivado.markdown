---
layout: post
title:  "Running Vivado on Linux (Ubuntu)"
date:   2015-05-02 12:00:00
categories: jekyll update
excerpt: This note shows how to run Vivado on Linux and shows how to fix a couple of issues with the installation. 
screenshot: note-3.jpg
note: 3
---

We just [installed Vivado]({% post_url 2015-05-02-2-installing-vivado %}). Now we're going to run it for the first time. 

Open a terminal and source this file `source /opt/Xilinx/Vivado/2015.1/settings64.sh`. Add it to your `~/.bashrc` file so it's run each time you launch a terminal. 

Make a directory for projects and launch vivado. The whole sequence is below.

{% highlight bash %}
source /opt/Xilinx/Vivado/2015.1/settings64.sh
mkdir ~/vivado
cd ~/vivado
vivado &
{% endhighlight %}

Unfortunately, I had some errors at first start-up. The following commands helped. 

{% highlight bash %}
sudo chmod 777 -R /opt/Xilinx/
sudo chmod 777 -R ~/.Xilinx/
{% endhighlight %}

Try again.

{% highlight bash %}
vivado &
{% endhighlight %}

Vivado starts up and we're ready to program!

![Run these commands]({{ site.url }}/assets/note-3/run-vivado-1.png)

![Run these commands]({{ site.url }}/assets/note-3/run-vivado-2.png)

[Previous Note]({% post_url 2015-05-02-2-installing-vivado %}) - [Next Note]({% post_url 2015-05-02-4-adding-board-files %})