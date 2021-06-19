# How to upload project Heroku

#### Deploy your app to Heroku site [DEMO View](https://aqueous-basin-57981.herokuapp.com/)

[Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python)

[developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Learn/Server-side)

[Youtube Tutorial](https://www.youtube.com/watch?v=vZTFEwfkTe8&list=PLlMOodDAsO4ytqbGWRIs34fs_bIKG9lXg&index=7)

#### Contents:

1. Deployment web app
2. Different Hosting
    1. https://www.pythonanywhere.com
    2. https://www.heroku.com
    3. DigitalOcean: https://m.do.co/c/ee79fbc29f9c
1. Git Installation
2. Heroku Configuration
3. Heroku CLI
4. Deploy to Heroku
 
#### Heroku Deployment Tasks:
```
1. Create a <Procfile> in root project or dir and write
   	web: gunicorn DJANGO_PROJ_NAME.wsgi --log-file -
2. Replace the <Project name> with actual project name
3. pipenv install gunicorn
4. pipenv install whitenoise
5. pipenv shell
6. heroku login
7. heroku create RANDOM_PRJ
8. heroku git:remote -a RANDOM_PRJ

    7. Open settings.py and write 
        1. ALLOWED_HOSTS = ['*']
	INSTALLED_APPS = 'whitenoise.runserver_nostatic',
	MIDDLEWARE = 'whitenoise.middleware.WhiteNoiseMiddleware',
    8. git add -A
    9. git commit -m "update heroku configuration"
    10. git push heroku master
    11. heroku ps:scale web=1
    
```

Reference:
1. Git Installation: https://git-scm.com/downloads
2. Heroku Server: https://www.heroku.com
3. Gunicorn: http://gunicorn.org
4. 
