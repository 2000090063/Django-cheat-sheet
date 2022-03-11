# Django-cheat-sheet

## Virtual Env
#### to install virtualenv
`pip install virtualenv`

#### to create virtualenv
`virtualenv <venv_name>`

#### to activate virtualenv
`source <venv_name>/bin/activate`

#### to deactivate virtualenv
`deactivate`

## Git Tutorial
#### initialize git
`git init`

#### add your local repository as remote for your main repository
`git remote add origin https://github.com/user/repo.git`

#### Verify new remote
`git remote -v`

#### to add uncommited files
`git add .`
or
`git add -A`

#### to commit
`git commit -m ""`

#### to pull
`git pull`

#### to push as master
`git push -u origin master`

## Django
#### to start a project
`django-admin startproject <project_name>`

#### to create an app
`python manage.py startapp <app_name>`

#### to run server
`python manage.py runserver`

#### to make migrations to db
`python manage.py makemigrations`

#### to complete migration
`python manage.py migrate`

#### to create superuser
`python manage.py createsuperuser`


## PostgreSQL
#### to start postgres in command line
`psql -U <user_name> <db_name>`

#### to view relations
`\dt`

#### to view users and their roles
`\du`

#### to change password
`\password postgres`


## Steps to add an app to the database
1. Create the app model in models.py file of that app
2. Add the app in the settings.py file of the project
    * app.apps.app_nameConfig
3. Create Migrations (python manage.py makemigrations)
4. Migrate (python manage.py migrate)
5. Add app to the admin
    * from .models import app
    * admin.site.register(app)

### License

- [MIT License](url) 

Copyright (c) 2022 Karthik Reddy Veluru

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

