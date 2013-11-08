---
layout: post
title:  "Add a second page a and link to it"
chapter: "one"
---

TODO: screenshots

Having a page is nice, but having more pages is more nice. So lets add another one.

## Challenge

Make a new page `kittens.html` and put a paragraph with "hello kittens" on it. Then add an image with a kitten. Finally, add a link from `index.html` to your new `kittens.html` and vice versa.

## How to do it

The first part should be well-know to you from the last lesson:

- make a new file called `kittens.html`
- remember the "paragraph" from last lesson? Make one and write "hello kittens" inside

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

Now we will add our first image:

- put img-tag below the paragrap

![]({{ site.baseurl }}/assets/images/create-repo-5.png)

The browser knows now that you want to habe an image displayed at this position. Be it doesn't know yet *what* image you want to see there. We have to tell it.

We do that by adding an *attribute*: the *source* of the file to display:

![](http://placekitten.com/g/500/300)

Sweet kitten, huh?

Now we want a link on our index page so we can go to the kittens anytime we want:

![]({{ site.baseurl }}/assets/images/create-repo-5.png)
SCREENSHOT: - add href to kittens-link on index

Goto your tab with yourusername.github.io and refresh. "To the kittens" should now be underlined and when you click on it, should take you to `kittens.html`.

Lastly, we want to be able to go back to the index from our kittens page, so let's add that:

![]({{ site.baseurl }}/assets/images/create-repo-5.png)
SCREENSHOT: - add go back link to index

### What did you do?

You used *Links* (originally "Hyperlinks", but it's not 1987 anymore) to connect to documents.

If you want, you can think of links as *portals*, which can take to *any* other place. It can be another site on the web, it can be another position in the same document.