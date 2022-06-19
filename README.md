# Django Url Admin Dashboard

## How to make and settings Admin in Django 
Django has provided all template like admin, auth, sessions, and etc as default project template.
All this template you can see at settings.py project in Application definition the name **INSTALLED_APPS**.
If you runserver at first time make project, you will find message about unapplied migration(s). 
So to apply that you just need write in command **python manage.py migrate**
And for database Django provide sqlite3.




The step:
- Make project use command **django-admin startproject <name_project>**.
- Open file settings.py in your project, scroll down and you will find INSTALLED_APPS. In there Django has provide template apps for admin, auth and etc.
- Run project server and you will find message about unapplied migration(s). 
- For migrations, use command **python manage.py migrate** . Then all migration will be done.
- Create account for admin use command **python manage.py createsuperuser**
- You will be asked to fill in username, email, and password.
- After that run server use command **python manage.py runserver**
- Open urls port http://127.0.0.1:8000/ and add /admin/ in end url
- Django will show Django admin. Enter the username, and password you add before.
- And TARAAA!! You enter in admin dashboard.
- Want change url from /admin/ to else name?
- Open file urls.py in project, in urlpattern change path /admin/ to name you want, example /zuri-admin/
- Run your server again and use the changed url.
- VOILAA!! Finishhh
