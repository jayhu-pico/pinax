# Quick Start

We strongly recommend running Pinax (or indeed, any Django) projects in a virtualenv:

```
pip install virtualenv
virtualenv mysiteenv
source mysiteenv/bin/activate
```

Once your virtualenv has been activated, install Django and use `django-admin.py` to create a new project based on the Account Pinax starter project:

```
pip install Django==1.8.4
django-admin.py startproject --template=https://github.com/pinax/pinax-starter-projects/zipball/account mysite -n webpack.config.js
```

Now install the requirements, initialize your database, load the default sites fixtures and run the dev server:

```
cd mysite
pip install -r requirements.txt
chmod +x manage.py
./manage.py migrate
./manage.py loaddata sites
./manage.py runserver
```

You now have a running Django site complete with account management and bootstrap-based templates.


@@@ Then add one more app