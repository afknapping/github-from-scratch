---
layout: post
title:  "A journal that makes sense"
chapter: "one"
---

TODO: screenshots, challenge

Remember when we said a repository is like a folder with a journal? Well, unitl now you didn't really write in that journal yourself. Github did that for you. That's the reason why your commit messages all look kind of the same:

    create index
    update index
    create kittens
    update kittens
    update kittens

and so forth.

While these messages tell you which file was changed, they don't tell you what exatly you did. More importantly, they don't tell you *why* you did it.

Imaginge you opened your personal journal from last year, and it featured entries like

    new day
    day was good
    new day
    day sucked
    watched movie

That's not very telling, is it? Why did the day suck? What movie did you watch? Was it any good?

So let's write a commit message that makes sense.


#### Challenge
Write a proper commit message that tells what the commit does and why it does it.


#### How to do it

A commit message shoud be phrased in first person present like this:

- verb (what is done)
- object (to whom)
- reason (why)

So you write from the point of view of the commit. It is easy and tempting to ommit the why part. But this will be the part that makes your changes accessible to other people. In the end they can read the code to see what changed. But unless you put comments within the code, they will never know the reasoning behind your decision.

Actually, you might not remember yourself two weeks in the future :)

So from now on, when you edit your files you will add a helpful commit message. Later your commit history should look more like this:

    
    fix typo on kittens.html
    change colors of headlines for better radability
    add image of barky to index because dogs are cute too

