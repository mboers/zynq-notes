---
layout: post
title:  "Installing Ubuntu 14.04 LTS on Mac with VMware Fusion"
date:   2015-05-02 12:00:00
categories: jekyll update
excerpt: To kick off this series of notes, we'll run through how to install Ubuntu 14.04 LTS on a Macbook Pro using VMware.
screenshot: note-1.jpg
note: 1
---

Install VMware Fusion, we're running Version 7.1.1. [Download from here](https://www.vmware.com/au/products/fusion)

Install Ubuntu 14.04 Trusty Tahir

{% highlight bash %}
sudo apt-get update
sudo apt-get remove --purge libreoffice*
sudo apt-get clean
sudo apt-get autoremove
sudo apt-get upgrade
{% endhighlight %}

[Next Note]({{site.baseurl}}/2-installing-vivado)
