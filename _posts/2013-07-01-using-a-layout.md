---
layout: post
title:  "Using a Layout"
chapter: "one"
---

We're nearly done to leave the port. One more thing.

#### Challenge
Use a <em>layout</em> which has a menu with links to both of your pages. Use that layout on both pages.

#### How to do it

So first we must create the layout. This is a special kind of page which determines how all your HTML pages should look like. Our motor *Jekyll* expects those layout files to be in a folder called `_layouts`. But how do we create a folder on GitHub?

This is as easy as creating a new file. Actually you start as if you wanted to create a new file, but you write the name of the folder in the name field and *do not click on OK yet!*

![]({{ site.baseurl }}/assets/images/layout-1.png)

Now type a *slash* `/` into the field and ta-daa:

![]({{ site.baseurl }}/assets/images/layout-2.png)

That folder will be created along with the file. Just keep typing in that field – our file needs to be called `default.html`:

![]({{ site.baseurl }}/assets/images/layout-3.png)

Edit that file and write a paragraph with "hello layout" and a line that only consists of "{&#8203;{ content }}"

![]({{ site.baseurl }}/assets/images/layout-4.png)

Now you need to tell Jekyll that your pages should *use* that layout. We do that by adding so called *front matter* to them. Open your index.html and then your kittens.html and edit them as shown:

![]({{ site.baseurl }}/assets/images/layout-5.png)

![]({{ site.baseurl }}/assets/images/layout-6.png)

Now go look at your page. They should look something like this:

![]({{ site.baseurl }}/assets/images/layout-7.png)

![]({{ site.baseurl }}/assets/images/layout-8.png)

Now add a *navigation menu* to the layout, where you keep links to all of your pages. Also, move the headline in there and delete it from the pages.

![]({{ site.baseurl }}/assets/images/layout-9.png)

![]({{ site.baseurl }}/assets/images/layout-10.png)

![]({{ site.baseurl }}/assets/images/layout-11.png)

Welcome to the internets!

## What did you just do?

Remember the data we put into the config file? Turns out each page can have its own set of data within *front matter*. Everything between the two three-minus lines is frontmatter. As with config, you can put all kinds of data within a page. Actually you're already using a specific *data format* called *Yaml*. Wasn't so hard so learn, that *data format*, right? Key, colon, value.

In your layout you now use a `site.title` which is read from the config file and a `page.title` which comes from the front matter in your pages. In case you are wondering: `<hr />` is a HTML Tag for printing out a simple horizontal line, or *horizontal rule*. 

The "{&#8203;{ content }}" is a very special variable and is a bit harder to understand. You tell a page to use layout in the front matter. But the layout mus also know where to render the *content* of the page. The two work together hand in hand. Delete "{&#8203;{ content }}" from your layout file and see what happens!

