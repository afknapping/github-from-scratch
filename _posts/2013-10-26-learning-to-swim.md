---
layout: post
title:  "Learning how to swim: HTML"
chapter: "one"
---

If you know your way around HTML, you can go through this real quickly. If not, just read on...

The browser can do more than just print a text from a file. It speaks its own language, called "HTML" (HyperText Markup Language). With HTML you can give the browser hints about the meaning of the different parts of your document. For example you can mark some text as a headline, a list or even a quote. 

#### Challenge
Make "hello world" a headline in your index.html. Then add a paragraph with the text "To the kittens!!1".

#### How to do it

- edit `index.html`
- change `hello world` to `<h1>hello world</h1>`
- add a new line with the content: `<p>To the kittens!!1!</p>`

![]({{ site.baseurl }}/assets/images/html-1.png)

Save the file, then open the browser tab with your yourusername.github.io page and refresh it. 

#### What it should look like

![]({{ site.baseurl }}/assets/images/html-2.png)

#### What did you do?

You used so called *tags* to *mark up* the text, so the browser knows what you want it to be. The `<p>` tag signals to the browser, that this is a normal *paragraph* of text, an `<h1>` is a *headline*.

You can imagine these tags as being like uniforms: it is not so relevant who the person in the Police uniform is. It is more important that she is a Police Officer.

For the browser it doesn't really matter what your headline says. It is more important that it knows you want it to be a headline.

Tags usually consist of an opening tag (`<p>`) and a closing tag (`</p>`) and exist for all kinds of things. Some examples are:

- Structured headlines (`<h1>, <h2>,.., <h6>`)
- Bullet point lists (`<ul>`) with bullet point items (`<li>`)
- Blocks of code examples (`<code>`)
- Cited text (`<blockquote>`)
- Images (`<img>`)
- Links (`<a>`)

...and there are many, many more. If you are interested in learning more about HTML, we later have a special task for you. For now these few examples should be enough to keep you going. 

But wait - there are two tags we should look at right now, as they are two of the foundation blocks of the internet! <a href="{{ site.baseurl }}/second-page/">Read about them on the next page</a>.





