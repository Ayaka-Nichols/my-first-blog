![Djangogirls](photos\Djangogirls.PNG)


# my-first-blog
****
This website enbles you to share your life as a diary and create and manage your online identity.


# Description
This is a repository that contains with the source code for the DjangoGirls Tutorials,
This tutorial, which is run by the organization DjangoGirls, aims to cover the fundamentals of using HTML, CSS, Python, and Django. 
<br>
You should be able to create your own working **blog** with the source code.


# Demo
On the top page, click + on the right top corner to make a new blog post.
![DjangogirlsDemo1](photos\DjangogirlsDemo1.png)
<br>
<br>
Then fill out the title, text, save, then voila! Now you have your first blog post appears.
![DjamgogirlsDemo2](photos\DjangogirlsDemo2.png)


# Requirement
****
- Windows 10 Home21H2
- HTML
- CSS
- Python 3.10.8
- Django~=3.2.10
- Visual Studio Code
- Virtual Environments (venv)
- Pythonanywhere
- GitHub


# Usage
****
### Here is a list of the procedures for setting up a blog.
<br>
<br>

Set up a virtual environment and Django
  <br>- Create folder "djangogirls" 
  <br>〈command-line〉
  ```
  > mkdir djangogirls
  > cd djangogirls
  ```
Create a virtual environment
 <br>〈command-line〉
  ```
  > python -m venv myvenv
  > Set-ExecutionPolicy -ExecutionPolicy　RemoteSigned -Scope Process
  > myvenv/Scripts/activate
  ```
Install django with pip
 <br>〈command-line〉
  ```
  (myvenv)> python -m pip install --upgrade pip
  ```
Create a first Django project
<br>〈command-line〉
  ```
  > django-admin.exe startproject mysite .
  ```
Make some changes on setting.py
 1. Set time zone
 <br>〈mysite/settings.py〉
  ```
  TIME_ZONE = 'Asia/Tokyo'
  ```
  2. Set language
  <br>〈mysite/settings.py〉
  ```
  LANGUAGE_CODE = 'ja'
  ```
  3.Set static file location
  <br>〈mysite/settings.py〉
  ```
  STATIC_URL = '/static/'
  STATIC_ROOT = os.path.join(BASE_DIR, 'static')
  ```
  4.Set host address
  <br>〈mysite/settings.py〉
  ```
  ALLOWED_HOSTS = ['127.0.0.1', '.pythonanywhere.com']
  ```
  5. Database settings
  <br>〈mysite/settings.py〉
  ```
  DATABASES = {
      'default': {
          'ENGINE': 'django.db.backends.sqlite3',
          'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
      }
  }
  ```


# License
****
An Attribution-ShareAlike 4.0 Creative Commons license is used for the Django Girls Tutorial. 

# Authors
****
- Ayaka Nichols
- Original author of the source code: Django girls

# References
****
- [Django Girls のチュートリアル](https://tutorial.djangogirls.org/ja/)
<br>
- [Documentation Django Girls Tutorial Note](https://linuxtut.com/en/c7ac38a69e0865a4bcd7/)


