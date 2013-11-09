---
layout: post
title:  "Linking pages"
chapter: "one"
---

Having a page is nice, but having more pages is more nice. So lets add another one.

<div class="challenge">
	<p><strong>Challenge</strong><br />
	Make a new page kittens.html and put a paragraph with "hello kittens" on it. Then add an image with a kitten. Finally, add a link from index.html to your new kittens.html and vice versa.</p>
</div>


#### How to do it

The first part should be well-known to you from the last lesson:

Start with adding a new file called `kittens.html`.
Remember the "paragraph" tag from last lesson? Make one and write "hello kittens" inside.

![]({{ site.baseurl }}/assets/images/html-3.png)

Now we will add our first image! For images we can use the `img` tag:

`<img />`

As you can see, this one consists of only one tag, unlike the paragraph or headline tags we used before. 
Place this image tag below the paragraph.

![]({{ site.baseurl }}/assets/images/html-4.png)

The browser now knows that you want to have an image displayed at this position. But of course it doesn't know yet *what* image you want to see there. We have give the browser some details.

We do that by adding an *attribute*: the *source* of the file to display, or in short, `src`.

![]({{ site.baseurl }}/assets/images/html-5.png)

![](http://placekitten.com/g/500/300)

Sweet kitten, huh? Awwwww.

Now we want a link on our index page so we can go to the kittens page anytime we want!

So switch over to the index.html file and edit it. To create a link, we use the `a` tag. And just like we did with the image we have to tell the browser where the link should link to with an attribute. In this case the attribute is called `href`.

![]({{ site.baseurl }}/assets/images/html-6.png)

Go to your tab with yourusername.github.io and refresh. "To the kittens" should now be underlined and when you click on it, should take you to `kittens.html`.

Lastly, we want to be able to go back to the index from our kittens page, so let's add a link there, too:

![]({{ site.baseurl }}/assets/images/html-7.png)

#### What did you do?

You used *Links* (originally "Hyperlinks", but it's not 1987 anymore) to connect documents.

If you want, you can think of links as *portals*, which can take you to *any* other place. It can be another site on the web, it can be another position in the same document.