---
layout: post
title:  "Installing Vivado"
date:   2015-05-02 12:00:00
categories: jekyll update
---

You'll find this post in your `_posts` directory - edit this post and re-build (or run with the `-w` switch) to see your changes!
To add new posts, simply add a file in the `_posts` directory that follows the convention: YYYY-MM-DD-name-of-post.ext.

This is cool. 

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

{% highlight verilog %}
module arbiter (
// Two slashes make a comment line.
clock      , // clock
reset      , // Active high, syn reset
req_0      , // Request 0
req_1      , // Request 1
gnt_0      , // Grant 0
gnt_1        // Grant 1
);
//-------------Input Ports-----------------------------
// Note : all commands are semicolon-delimited
input           clock               ;
input           reset               ;
input           req_0               ;
input           req_1               ;
//-------------Output Ports----------------------------
output        gnt_0                 ;
output        gnt_1                 ;
{% endhighlight %}


Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll's GitHub repo][jekyll-gh].

![My helpful screenshot]({{ site.url }}/assets/getting-started-1.png)

[jekyll-gh]: https://github.com/mojombo/jekyll
[jekyll]:    http://jekyllrb.com

