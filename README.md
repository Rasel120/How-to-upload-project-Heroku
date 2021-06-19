# How to upload project Heroku

#### Deploy your app to Heroku site [DEMO View](https://aqueous-basin-57981.herokuapp.com/)

[Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python)

[developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Learn/Server-side)

[Youtube Tutorial](https://www.youtube.com/watch?v=vZTFEwfkTe8&list=PLlMOodDAsO4ytqbGWRIs34fs_bIKG9lXg&index=7)

#### Contents:
1. Deployment web app
2. Different Hosting
    1. [Pythonanywhere](https://www.pythonanywhere.com)
    2. [Heroku](https://www.heroku.com)
    3. [DigitalOcean](https://www.digitalocean.com)
1. Git Installation
2. Heroku Configuration
3. Heroku CLI
4. Deploy to Heroku
 
#### Heroku Deployment and Command Tasks:
```
1. Create a <Procfile> in root project or dir and write 	NB: capital letter <P> for Prockfile
   	web: gunicorn Project_Name.wsgi --log-file -
2. Open project settings.py  Add and Edit
        ALLOWED_HOSTS 	= ['*']
	INSTALLED_APPS 	= 'whitenoise.runserver_nostatic',
	MIDDLEWARE	= 'whitenoise.middleware.WhiteNoiseMiddleware',
	
3. pipenv install gunicorn
4. pipenv install whitenoise
5. pipenv shell
6. heroku login   or	heroku login -i
7. heroku create  or   heroku create 'Url name'
8. heroku git:remote -a Url_name

9. git init
10 git add -A
11 git commit -m "write your commet"
12 git push heroku master
13 heroku ps:scale web=1   or	 heroku ps:scale web=0
    
```

Reference:
1. Git Installation: https://git-scm.com/downloads
2. Heroku Server: https://www.heroku.com
3. Gunicorn: http://gunicorn.org

