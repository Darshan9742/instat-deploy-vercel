# Deploying Instat to Heroku
## Clone of the project folder is made
### Step 1 - Installing whitenoise & gunicorn through pipenv

Commands 
- `pipenv install whitenoise`
- `pipenv install gunicorn`

### Step 2 - Creating `Procfile` inside root directory manually

Copy this code into that file `web: unicorn instatMain.wsgi`

### Step 3 - Create `requirements.txt`

Firstly, activate the virtual env by entering command - `pipenv shell`
then run `pip freeze > requirements.txt`

### Step 4 - Create a prvt github repository and push code there

commands - 
- `git init`
- `git add .`
- `git commit -m "django-deploy"`
- `git branch -M main`
- `git remote add origin https://github.com/thekaranatic/instat-deploy.git`
- `git push -u origin main`