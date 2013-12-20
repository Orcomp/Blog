---
layout : post
title : Simple Blogging
category : Simple
tags :
  - Blog
  - gh-pages-blog
  - Jekyll
  - Simple
---

I was looking for low ceremony, version controlled blogging framework, and found two good contenders [gh-pages-blog](https://github.com/thedereck/gh-pages-blog/) and [Octopress](http://octopress.org/)

I ended up choosing [gh-pages-blog](https://github.com/thedereck/gh-pages-blog/) as it looked like the easiest to setup.

# Installation

## gh-pages-blog

- Create a new repository on your github account called \"Blog\". (For example this is mine: [https://github.com/Orcomp/Blog](https://github.com/Orcomp/Blog))
- Clone the repository to your computer.
- Copy the files from the [gh-pages-blog](https://github.com/thedereck/gh-pages-blog/) repository to your \"Blog\" repository. (i.e. you will probably need to clone the gh-pages-blog repo to another folder and then copy the files across.)
- On your computer \"Blog\" repository run the following command to create a \"gh-pages\" branch:


    	git checkout --orphan gh-pages


- Modify the config.yml to reflect your own settings. (i.e. change the author name and URL address etc.)
- Commit the files to your local repo, then push your commit to github. Within the next 10 mins you should be able to navigate to http://username.github.io/Blog. You will see a \"Hello World\" post.
- To add new posts follow the instructions found [here](http://thedereck.github.io/gh-pages-blog/user-manual/getting-started.html).

Once you have this working, you will realise that in order to preview your blog posts you have to push the commits to github, which is not ideal. Instead you can install Jekyll on your own computer which will render your blogs the same way github will, without having to make a commit.

The next section will show you how to install the necessary software to get your blog running on your local computer within 10 mins.

# Installing Jekyll the easy way

If you don\'t have [Chocolatey](http://chocolatey.org/) installed on your computer, then install it first. It makes everything else really simple and Chocolatey only takes 10 secs to install anyway.

Simply open a command prompt and copy the text below and press enter:

    @powershell -NoProfile -ExecutionPolicy unrestricted -Command \"iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))\" && SET PATH=%PATH%;%systemdrive%\chocolatey\bin

A few seconds later, Chocolatey will be installed.

Then install Ruby using Chocolatey. (I found ruby 1.9 to work best)
At the command prompt type:

	cinst ruby1.9

This will create a \"C:\ruby190\" directory with ruby binaries in it.

Then install ruby DevKit.
At the command prompt type:

	cinst ruby.devkit

This will create a \"C:\DevKit\" directory.

Then follow the instructions on this page: [http://flatshaded.com/2013/05/installing-jekyll-on-windows/](http://flatshaded.com/2013/05/installing-jekyll-on-windows/) (NOTE: you already have devkit installed, so all you need to do is initialise the config.yml, then edit the file by adding the location of your ruby installation at the end of the file with a leading \'-\' i.e. \"- C:\ruby190\". Then run the command `ruby dk.db install`.)

Then at the command prompt type in:

     gem install bundler

Finally to install Jekyll follow the instructions found in point 3 of this page: [https://help.github.com/articles/using-jekyll-with-pages](https://help.github.com/articles/using-jekyll-with-pages).
Which is shown in the image below:

![Jekyll Installation](/img/SimpleBlogging/InstallJekyll.png)

If you followed the instruction above you will have:

- Created a Gemfile (with no extension) in your base repository and added the following lines to it:
       source 'https://rubygems.org'
	   gem 'github-pages'

- Run the command `bundle install` at the command prompt in your repository.

Just to be on the safe side you should also run:

     bundle update

You can now run the Jekyll server. Execute the following command in your Blog repository:

    bundle exec jekyll serve

then point your browser to: \"http://localhost:4000\"


# Tips

- Since Jekyll 1.4.2. You need to escape double quotes, single quotes and square brackets etc. 
i.e.

       \" and \' and \[  \]

- If you want Jekyll to automatically update your blogs as you edit the markdown files then start it using this command:

      jekyll serve --watch

NOTE: For some reason `bundle exec jekyll serve --watch` does not work.

- If the Jekyll server won\'t start, it probably means it cannot parse your blog posts. i.e. there is a formatting error it can\'t resolve. In this case start the server with:

      jekyll serve --watch --trace

in order to find out where the error is occurring.

- Create a batch file to start the server.

- To ensure your version of Jekyll is always in sync with github\'s, run `bundle update github-pages`.

# Links

Here are some useful links:

- [Jekyll](http://jekyllrb.com/) website with documentation
- [Octopress](http://octopress.org/) Very popular blogging framework for hackers.
- [Getting Started with gh-pages-blog](http://thedereck.github.io/gh-pages-blog/user-manual/getting-started.html)
- [Using Jekyll with pages](https://help.github.com/articles/using-jekyll-with-pages) Lots of valuable tips on this page.