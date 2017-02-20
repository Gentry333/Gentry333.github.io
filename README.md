# A Jekyll Theme with Bootstrap 4 integration

## Install

NOTE: Once I'm happy with the final configuration, I'll create a gem file. 
For now:

1.Simply clone the website with git to wherever you want.

2.Than run "bundle install" in the directory to ensure all the dependencies are met and the correct gem versions are installed.

3.Modify the global settings in /data/global.yml to match your own (as needed):

- for the 'url' setting, I added one for local development (127.0.0.1:4000), and another for when I upload to a production server (simply uncomment and recomment the other at publishing time, than switch back to the local one to continue any modification).

- change any of the Social media links to your own as needed.

NOTE: careful editing any yml files as they take indentation into account (spaces).S

4.Run "bundle exec jekyll serve" to build and host the site.


#### Also: 
-  the bootstrap javascript settings, font awesome, and jquery are linked to a remote CDN. You can modify those address if needed (they are located in the _includes/head.html).

-  The Bootstrap 4 SCSS files are installed locally in "_sass/bootstrap". Everything is loaded by default. If you would only like to load specific bootstrap files instead of everything, than edit the imports in 'css/main.scss'

-  To over-ride the bootrap base SCSS variables, modify them in '_sass/_variables.scss' (to make upgrading to a newer bootstrap version easier).




### Modify the frontpage image?

- the font page image is located in the img folder (BG_nice_image.jpg). Simply overwrite it leaving the name the same. Or change the name of it in the /_layouts/front.html file.

### How are the images set on the front page blog teasers?

- Each blog post on the front page will put an image that is the name of the title of the blog post. i.e. Whatever you put beside 'title:' in your posts, put an image of the same name in jpg format in the /img/posts folder (see the other post examples as to where you put the title. It must be in the "Front Matter" at the top of the file, between the '---'').

#### You can change the length of the frontpage teaser and the title max length at:
- inside the /_layouts/front.html
-  post.title | strip_html | truncatewords:5
-  post.content | strip_html | truncatewords:75


## Demo

You can see a live demo of the site at [https://gentry333.github.io](https://gentry333.github.io)


## What is this?

This is **a theme I'm working on that uses Jekyll's static site generator. I made it in order to integrate Jekyll with Bootstrap-4** so I could test any new features as Bootstrap 4 transitions from alpha to beta.


Jekyll is a simple and blog-aware static site generator built in Ruby. In laymen terms, it's just a tool to let you have **all the cool features of a full-blown CMS without having to worry about managing a database**. This means hosting is *extremely easy* and *scalable* since all you're doing is managing a bunch of files.

You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](http://jekyllrb.com/)

You can find the source code for Jekyll at [jekyll](https://github.com/jekyll/jekyll)









