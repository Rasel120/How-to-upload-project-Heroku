# How to upload Heroku

#### Deploy your Pytho Project into Heroku site [DEMO View](https://aqueous-basin-57981.herokuapp.com/)

#### Heroku Deployment and Command Tasks:
```
1. Create a <Procfile> in your root project or dir and write 	NB: Capital letter <P> for Procfile
   	web: gunicorn Project_Name.wsgi --log-file -
2. Open project settings.py and Add or Edit
        ALLOWED_HOSTS 	= ['*']
	INSTALLED_APPS 	= 'whitenoise.runserver_nostatic',
	MIDDLEWARE	= 'whitenoise.middleware.WhiteNoiseMiddleware',
3. Command Work:	
	1. pipenv install gunicorn
 	2. pipenv install whitenoise
 	3. pipenv shell
 	4. heroku login   or	heroku login -i
 	5. heroku create  or   heroku create 'Url name'
 	6. heroku git:remote -a Url_name

	7. git init
	8. git add -A
	9. git commit -m "write your commet"
 	10. git push heroku master
	11. heroku ps:scale web=1   or	 heroku ps:scale web=0
	
NB: You have to need install Gitbash,heroku software from there site
    
```

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

#### Reference:
[Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python)

[Youtube Tutorial](https://www.youtube.com/watch?v=vZTFEwfkTe8&list=PLlMOodDAsO4ytqbGWRIs34fs_bIKG9lXg&index=7)

1. Git Installation: https://git-scm.com/downloads
2. Heroku Server: https://www.heroku.com
3. Gunicorn: http://gunicorn.org

