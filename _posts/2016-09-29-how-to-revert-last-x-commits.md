---
layout: post
title: How to revert last X commits
source: http://ohshitgit.com/
---

{% highlight sh %}
$ git reflog
# you will see a list of every thing you've done in git, across all branches!
# each one has an index HEAD@{index}
# find the one before you broke everything
$ git reset HEAD@{index}
# magic time machine
{% endhighlight %}


You can use this to get back stuff you accidentally deleted, or just to remove some stuff you tried that broke the repo.
