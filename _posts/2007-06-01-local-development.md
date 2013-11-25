---
layout: post
title:  "Local Development"
chapter: "two"
---

If you have written code before, you might have done it in a text editor on your own machine instead of online. To do so, we need to download our repository and synchronize local changes to GitHub.

#### Challenge
*Clone* your GitHub repository to your computer and keep your repositories synchronized.


#### Installing stuff

Let's start by installing the tools needed. After that we have a look on how to keep your repositories in sync.

##### GUI Tools for Git and GitHub with a "normal" click-interface

GitHub is making its own GUI tools for Mac and Windows. You can download them here:

- [GitHub for Mac](http://mac.github.com/)
- [GitHub for Windows](http://windows.github.com/)

There many many other clients available than those by GitHub. The Git documentation page holds [a short list](http://git-scm.com/downloads/guis) and even more can be found through [the Delicious of Matthew McCullough](https://delicious.com/matthew.mccullough/gui,git).

If you are a **Linux** user, you might want to check out this answer on Stack Overflow: [Git GUI client for Linux](http://stackoverflow.com/questions/1516720/git-gui-client-for-linux/1518844#1518844).

##### Code editors

We recommend Sublime Text, which is widely used by many coders of all languages, has a rich ecosystem of plugins and themes and is available for Mac, Windows and Linux.

- [Sublime Text](http://www.sublimetext.com/)

Sublime Text is free to try, but you need to buy a license after 30 days. If you want to go with something completely free/libre, try

- [gedit](https://projects.gnome.org/gedit/)

##### The Command Line

If you want to use Git in the terminal, it helps to have done your first steps in [Bash](https://en.wikipedia.org/wiki/Bash_\(Unix_shell\)) before. We would recommend you to start with [The CLI Crash Course on *Learn Code The Hard Way*](http://cli.learncodethehardway.org/).

To install Git without a GUI tool, download it here: [Git Book](http://git-scm.com/downloads).


#### Working locally on your GitHub project

##### Check your Git version
To verify that Git is correctly installed on your system, open a terminal window and type the following (without the dollar sign, that should already be there):

	$ git --version 

You should see a version number now. If there is an error, please see above to install Git.

Now tell git your name and email address, so that it can add this info to the commits you make. Your email address for Git should be the same one associated with your GitHub account. You propably want to use the same name you use on GitHub too.

	$ git config --global user.name "Your Name"
	$ git config --global user.email "your_email@example.com"

##### Obtain your local copy

Copying a repository from another location is called *cloning*. 

Take a look at your repository on GitHub. In the sidebar to the right there should be a field with an URL, labeled "clone URL". You can use the "HTTP clone URL" for now, but you should read about the details which can be found if you click on the small question mark.

If you use the GitHub GUI, you can just click on "Clone in Desktop". On the terminal, you first change to the folder where you want to put your project files to be, for example:

	$ cd /Users/yourname/projects

Then copy the URL shown on your GitHub repository and type the following in your terminal (replace \<url> with that URL):
	
	$ git clone <url>

Git will now add a folder for your repository and copy all the files into it. Besides your project files there also will be a hidden folder `.git`. That's were Git stores everything it needs for keeping the version history.

##### Make changes

Did you create a `README.md` for your repository? If not, do so now locally. While a readme file isn't a required part of a GitHub or Git repository, it is a very good idea to have one. Most projects on GitHub have one and in it you'll find a description of the project and some documentation such as how to install or use it. In this case you might want to add some information about this OpenTechSchool course.

Open the `README.md` in your text editor, add a link to the course material and save the file.
Now we want to *stage* it, adding it to the list of files to be committed. Then we *commit* it with a commit message. In the terminal do the following:

	$ git add README.md
	$ git commit -m 'add link to the OpenTechSchool course material'

Your edit is now ready to be pushed back to GitHub.
	
	$ git push origin master

Git will then ask for your GitHub username and password. "origin master" is the name of the *branch* you checked out. We will explain that in more detail later.

Now if you look at your repository on GitHub, you will see your README has been updated. In your commit history you will find your commit with message and everything.

Congratulations!

###### Branch
TODO


----
On codeschool there is a nice small Git learning course. If you want to experiment some more, you might want to try it at [Try Git](http://try.github.io/levels/1/challenges/1).



