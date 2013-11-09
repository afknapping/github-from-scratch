---
layout: post
title:  "Using a Layout"
chapter: "one"
---

We're nearly done to leave the haven. One more thing.

## Challenge

Use a *layout* which has a menu with links to both of your pages. Use that layout on both pages.

## How to do it

So first we must create the layout. Our motor *Jekyll* expects those to be in a folder called `_layouts`. But how do we create a folder on Github?

Create a new file, write the name of the folder in the name field but *do not click on OK yet!*

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

Now type a *slash* `/` into the field and ta-daa:

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

That folder will be created along with the file. Just keep typing in that field – our file needs to be called `default.html`:

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

in that file, put a paragraph with "hello layout" and a line that only consists of "`{{ content }}`"

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

Now you need to tell Jekyll that your pages should *use* that layout. We do that by adding so called *front matter* to them:

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

Now go look at your page. They should look something like this:

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

Now add a *navigation menu* to the layout, where you keep links to all of your pages. Also, move the headline in there and delete it from the pages.

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

Welcome to the internets!

## What did you just do?

Remember the data we put into the config file? Turns out each page can have it's own set of data within *front matter*. Everything between the two three-minus lines is frontmatter. As with config, you can put all kinds of data within a page. Actually you're already using a specific *data format* called *Yaml*. Wasn't so hard so learn, that *data format*, right? Key, colon, value.

The `{{ content }}` is a very special variable and is a bit harder to understand. You tell a page to use layout in the front matter. But the layout mus also know where to render the *content* of the page. The two work together hand in hand. Delete `{{ content }}` from you layout file and see what happens!

And with this...




