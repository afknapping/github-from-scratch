---
layout: post
title:  "Jekyll in action: make a blog"
chapter: "two"
---

A static site is cool – but having a blog where you can regularly write is better!

#### Challenge

Write your first two posts and add a linked list of all posts to your index.


#### How to do it

Create a new directory `_posts` and in that a file `2013-11-30-my-first-post.md`.

Write this into the post:

    ---
    title: my first post
    layout: default
    ---
    hello world

Now open `yourusername.github.io/2013/11/30/my-first-post.html`. Awesome, huh? There it is! The thing is, that is has no headline. So we will make a special layout for blogposts:

Create a new file `post.html` in the `_layouts` folder. Put this inside the file:

    <h1>{{ page.title }}</h1>
    {{ content }}

In your post, change `layout:` from `default` to `post`.


If you now go back to `yourusername.github.io/2013/11/30/my-first-post.html` you should have your headline generated from what you entered behind `title:` on top.

Let's make a second post `2013-11-30-my-second-post.md` with this inside:

    ---
    title: my second post
    layout: post
    ---
    hello kittens

Only one thing left missing. We want to have a list of all our blogposts on our index, right? Put this into your `index.html`:
    
    <ul>
        {% raw %}{% for post in site.posts %}
            <li><a href="{{ post.url }}">{{ post.title }}</a></li>
        {% endfor %}{% endraw %}
    </ul>

`yourusername.github.io/` should now feature the two posts you already wrote. But the great part is: any post you add will automatically appear in this list! Awesome, huh?

Actually, by using {% raw %}{% for post in site.posts %}{% endraw %} you did your first bit of programming! You *iterated over an array*. But that is something for another course :)

## What did you just do?

You used [Jekyll to makes pages from your blogposts](http://jekyllrb.com/docs/posts/) and [Liquid](https://github.com/shopify/liquid/wiki/Liquid-for-Designers) to generate headlines and a list of posts. Follow these links to learn about it.

## And what about that ".md" file extension?

You discovered one the secret superpowers of the web: Markdown.

Markdown provides you with a small subset of HTML-Tags – without having to write the tags! That's right. Here's an example that should get you started:

    ## A sub headline

    this is a paragraph. 
    Here is an image: 
    ![more kittens](http://placekitten.com/g/200/200). 
    [This is a link](http://www.nyan.cat/).

    - and this
    - is a
    - list

will become

    <h2>A sub headline</h2>

    <p>
    this is a paragraph. 
    Here is an image: 
    <img src="http://placekitten.com/g/200/200" alt="more kittens">. 
    <a href="http://www.nyan.cat/">This is a link</a>.
    </p>

    <ul>
    <li>and this</li>
    <li>is a </li>
    <li>list</li>
    </ul>

Just try Markdown out in your posts and [read more about it at the creator's site](http://daringfireball.net/projects/markdown/basics).


