https://devcenter.heroku.com/articles/getting-started-with-django
https://devcenter.heroku.com/articles/heroku-postgresql

```
sudo -u postgres createdb sayitlike

# settings.py
# Parse database configuration from $DATABASE_URL
db = {'username': 'postgres',
      'password': 'beffy44',
      'name': 'books',}

DATABASES['default'] = dj_database_url.config(
                        default='postgres://%s:%s@localhost:5432/%s' % (
                                db['username'], 
                                db['password'], 
                                db['name']))
```
