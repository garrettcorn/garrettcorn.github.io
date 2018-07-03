---
layout: post
title:  "Hello World!"
date:   2018-05-30 20:05:04 -0700
categories: jekyll update
---

This post will mainly be for personal reference, but it may help you out along the way. This post will simply
contain information about updating, adding post, and a few other general maintenance tid bits for GitHub Pages
using Jekyll.

LaTex to MarkDown conversions. I'll likely do a full post with all of the steps at a later date, but for now this will have to do.
This assumes the user is using Linux, Ubuntu 18.04 to be exact, sorry Mac and Windows, well not really but I digress.
* Write post in LaTeX. Can use texstudio `bash sudo apt install -y texstudio`
* Use pandoc to convert from LaTeX to MarkDown
  * Install pandoc `sudo apt install -y pandoc`
  * Convert a LaTeX post with something similar to `pandoc -s post.tex -o post.md`
* Rename or give a proper name in the previous step and to the `_posts` folder

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for previous post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hello(name)
  puts "Hello #{name}"
end
print_hello('World!')
#=> prints 'Hello World!' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
