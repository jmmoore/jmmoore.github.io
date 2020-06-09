---
layout: "post"
title: "CSS: Center Multiple Lines on a Shared Character"
description: "One solution to an interesting problem"
categories: ["webdev"]
tags: ["webdev", "css", "tutorials", "html5"]
---

In my work sprucing up [College Hill Creative](http://collegehillcreative.com/)'s homepage, I discovered something that bothered me at the bottom of each page. The roster was formatted like so:


```html
<p style="text-align: center">
    Name Number One | Title Number One<br/>
    Slightly Shorter | Shorter Title<br/>
    Tiny | Tiny<br/>
</p>
```

It rendered like this:

<p style="text-align: center">
    Name Number One | Title Number One<br/>
    Slightly Shorter | Shorter Title<br/>
    Tiny | Tiny<br/>
</p>

The fact that the text wasn't centered on the pipes bothered me significantly, and I went to work trying to fix the issue.

My initial searches led me to attempt to maintain whitespace inside of the p element. This got close, but was too finicky and lacked precision. After spending some additional time trying in vain to solve the problem on my own, I reached out to the [devICT](https://devict.org/) Slack channel for help.

[Barrett Morgan](http://www.barrettmorgandesignllc.com/) offered the following suggestion:

>@jmmoore you might try wrapping each side of the pipe in divs that are 50% wide. Then right aligning one side and left aligning the other...

He provided some sample code as well:

<iframe width="100%" height="300" src="//jsfiddle.net/jmmoore/5Lp1Lq8u/embedded/html,css,result/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

It rendered relatively close to the way I wanted but the centering still wasn't exactly where I wanted it to be. However, I took his suggestions and spent some time trying different margin combinations. After some experimentation, putting the pipe character inside its own classed div did the trick.

The final version that works is on JSFiddle, embedded below:
<iframe width="100%" height="300" src="//jsfiddle.net/jmmoore/5suyaqto/embedded/html,css,result/" allowfullscreen="allowfullscreen" frameborder="0"></iframe>

This doesn't strike me as a particularly elegant solution, so if you have solved this problem in a different way, please reach out to me on [Twitter](https://twitter.com/jmmoore_)!