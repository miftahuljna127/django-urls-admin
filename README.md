# Django Url Admin Dashboard

## How to make and settings Admin in Django 
Django has provided all template like admin, auth, sessions, and etc as default project template.
All this template you can see at settings.py project in Application definition the name **INSTALLED_APPS**.
If you runserver at first time make project, you will find message about unapplied migration(s). 
So to apply that you just need write in command **python manage.py migrate**
And for database Django provide sqlite3.




The step:
- Make project use command **django-admin startproject <name_project>**.
2. Open file settings.py in your project, scroll down and you will find INSTALLED_APPS. In there Django has provide template apps for admin, auth and etc.
4. Run project server and you will find message about unapplied migration(s). 
5. For migrations, use command **python manage.py migrate** . Then all migration will be done.
6. Create account for admin use command **python manage.py createsuperuser**
8. You will be asked to fill in username, email, and password.
9. After that run server use command **python manage.py runserver**
10. Open urls port http://127.0.0.1:8000/ and add /admin/ in end url
11. Django will show Django admin. Enter the username, and password you add before.
12. And TARAAA!! You enter in admin dashboard.
13. Want change url from /admin/ to else name?
14. Open file urls.py in project, in urlpattern change path /admin/ to name you want, example /zuri-admin/
15. Run your server again and use the changed url.
16. VOILAA!! Finishhh
