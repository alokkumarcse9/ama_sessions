### 1. What is CSRF?

CSRF stands for Cross-Site Request Forgery. It is a security attack where someone tries to make a logged-in user perform an unwanted action. Django protects against this using a CSRF token.


### 2. What is `reverse()` in Django?

`reverse()` is used to get the actual URL from the URL's name. Instead of writing the URL directly, we provide its name, and Django gives us the corresponding URL.


### 3. What is the difference between the `path` in settings and the `path` in URLs?

In `urls.py`, `path()` is used to define the routes of a website. In `settings.py`, paths are generally used to specify the location of files and folders. So, one is for web routes and the other is for file locations.


### 4. What is `include()` in Django?

`include()` is used to connect an app's `urls.py` with the main project's `urls.py`. It helps us organize URLs by keeping the URLs of each app in a separate file.


### 5. What is an atomic transaction?

An atomic transaction means that multiple database operations are treated as one unit. Either all operations are completed successfully, or if something fails, all the changes are rolled back.

In simple words, **it is all or nothing**.


### 6. What is `Promise.all()`?

`Promise.all()` is used when we have multiple promises and want to wait for all of them to complete. If all promises succeed, we get all their results. If even one promise fails, `Promise.all()` also fails.


### 7. What is the difference between `migrate` and `makemigrations`?

`makemigrations` creates migration files based on changes in our Django models.

`migrate` applies those migration files to the database.

* `makemigrations` → Create migration
* `migrate` → Apply migration


### 8. What is `DictReader`?

`DictReader` is used to read CSV files in Python. It reads each row as a dictionary, where the column names become the keys.

For example, instead of accessing a value using an index, we can use:

```python
row["name"]
```

So it makes CSV data easier to work with.


### 9. What are ORM queries?

ORM stands for Object-Relational Mapping. Django ORM allows us to interact with the database using Python code instead of writing SQL queries directly.

For example:

```python
User.objects.filter(age=20)
```

Django converts this into the required SQL query behind the scenes.


### 10. How do you create a project in Django?

We can create a Django project using:

```bash
django-admin startproject myproject
```

Then we enter the project directory:

```bash
cd myproject
```

And start the development server:

```bash
python manage.py runserver
```

If we want to create an app inside the project, we use:

```bash
python manage.py startapp myapp
```

So basically, **`startproject` creates the project and `startapp` creates an application inside the project.**
