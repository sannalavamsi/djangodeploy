# django-deploy

Buy & Sell E-Commerce site: 

https://vamsi-mysite.herokuapp.com/myapp/products/

--> Steps to Upload Django Project into Heroku :

1. pip install gunicorn - The Gunicorn is a Python Web Server Gateway Interface HTTP server.
2. pip install whitenoise - WhiteNoise allows your web app to serve its own static files, 
                            making it a self-contained unit that can be deployed anywhere without relying on nginx, 
                            Amazon S3 or any other external service. 
                            (Especially useful on Heroku, OpenShift and other PaaS providers.)
3. Create requirements.txt - pip freeze > requirements.txt
4. Craete runtime.txt - web: gunicorn mysite.wsgi --log-file -
5. Create Procfile - python-3.10.5
6. Create .gitignore - add env/  , so that while pushing into GitHub env file is ignored.

 --> Git:
 
 Git is a DevOps tool used for source code management. 
 It is a free and open-source version control system used to handle small to very large projects efficiently. 
 Git is used to tracking changes in the source code, enabling multiple developers to work together on non-linear development.
 
 --> Uploading Source Code into GitHub by using Git.
 
 Terminal :
 
 1. cd desktop/mysite
 2. git inti
 3. git commit -m "first commit"
 4. git add .
 5. git branch -m main
 6. git remove add origin http://....
 7. git config user.name "..."    #GitHub
 8. git config user.email "..."   #GitHub
 9. git push -u origin main
 
#GitHub Password is asked and you need to give the Token insead
   1. GitHub  / settings
   2. Developer settings
   3. Personal token access
   4. Create token
 
 --> If Source is Modefied and want to upload to GitHub Repository follow this Steps:
 
 1. git status
 2. git add .
 3. git commit -m "comment//.."
 4. git push origin main
 
 --> settings.py
 1. DEBUG = False
 2. ALLOWED_HOSTS = ['vamsi-mysite.herokuapp.com','127.0.0.1']
 
 --> Heroku
 1.settings/ Add buildpack/ python
 
