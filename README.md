
The Django Hub
======

## Introduction 

**The Django Hub** is a blog application I designed and deployed in Django, using
PythonAnywhere to host it. It's main purpose is to share my knowledge of the Django 
framework as I learn, and to implement technical features of Django so I can learn 
even more.
It is available at https://spiderflocks.pythonanywhere.com.
Thanks for checking it out! 

## How I made it

* I started the web app in the project folder for my site, by running 
  `python manage.py startapp blog` in the mysite folder.

* After this I added `blog` to my `INSTALLED_APPS` in the `settings.py` file.

* Then I implemented a `class` named `Post` in the models folder of the blog app,
  and I created all the attributes necessary for it to be a readable blog post.

* I created an admin panel so I could create a post. I used the Django inbuilt
  admin interface to do this.

* I imported the `Post` class from the models folder to the `admin.py` file in 
  the blog directory, and then I created the first post of the blog.

* After I finished with the `models` directory, I continued to build the `views`.
  I used `ListViews` and `DetailView` for this. These two are a subclass of 
  generic class-based views.
  
* Then I mapped the urls to the views I had created. I did this creating an
  `urls.py` file in my `blog` directory, and using the path function.
  
* After this I was ready to start creating my blog's templates, so after creating
  a directory called `templates` and adding the route to it in the `settings.py` 
  file, I proceeded to add the `base.html`, `index.html`, `sidebar.html` and 
  `post_detail.html` files to this directory. 
  
* I used the **Bootstrap** CSS framework for the User Interface, and the customized
  font. I added the CSS rules at the beginning of the `base.html` file, and I started
  with this file so I could configure the *navbar* and the *footer* first, as I was 
  going to use them in all of the pages.
  
* The `index.html` file (the home page) inherits from the `base.html` file. The 
  `sidebar.html` file was injected into `base.html` too, so I could make it globally 
  available for pages inheriting from `base.html`.
  
* Finally, `post_detail.html` inherits from `base.html` too, and it's the template
  for the detailed views of the posts.

## Last words

I hope you have enjoyed this README and that it was useful to you! I invite you to 
visit **The Django Hub** anytime you want. Thank you for reading :)
