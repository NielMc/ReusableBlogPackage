===== Blog =====
Blog is a reusable authorization app for Django
Detailed documentation is in the "docs" directory.
To install:
pip install git+https://github.com/NielMc/ReusableBlogPackage
To update:
pip install git+https://github.com/NielMc/ReusableBlogPackage --upgrade
Add the following line to your requirements.txt file:
git+https://github.com/NielMc/ReusableBlogPackage


Quick start -----------
1. Add "reusable_blog" to your INSTALLED_APPS setting like this::
    INSTALLED_APPS = (         ...         'reusable_blog', 'disqus'  )


2. Run `python manage.py makemigrations and migrate`.

3. Add url(r'^blog/', include('reusable_blog.urls')), to your urls.py file.

4.Add the blogs css::
<link rel="stylesheet"href="{%static"css/blog.css"%}">

5.Add a link to the blog in the base.html
<li><a href="/blog/">OurBlog</a></li>

6.Visit http://127.0.0.1:8000/blog/ to view the blogs you create.


