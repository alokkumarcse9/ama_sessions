### 1. What is UTF-8?
UTF-8 is a character encoding standard used to represent text. It can represent almost all characters and symbols from different languages. It is the most commonly used encoding for web pages and supports ASCII characters as well.

### 2. What is `render()`?
`render()` is a Django shortcut used to return an HTML page as an HTTP response. It combines a template with context data and sends the rendered HTML to the browser.

```python
return render(request, "home.html", {"name": "Alok"})
```

### 3. What is server-side authorization?
Server-side authorization checks whether a user has permission to perform a particular action or access a resource. It is performed on the server, so users cannot bypass it by modifying frontend code or requests.

### 4. What is `DEBUG=True` in development and `DEBUG=False` in production?
`DEBUG=True` enables detailed error messages and debugging information, which is useful during development. `DEBUG=False` hides sensitive error details and should be used in production for security.

### 5. What is a QuerySet?
A QuerySet is a collection of database objects returned by Django's ORM. It allows us to retrieve, filter, sort, and manipulate database records without writing raw SQL.

```python
Article.objects.filter(category="Technology")
```

### 6. What is a callback, and why do we use it?
A callback is a function passed to another function as an argument, which is executed later when a specific task or event occurs. We use callbacks for handling asynchronous operations, events, and executing code after another operation finishes.

```javascript
function greet(name, callback) {
    callback(name);
}
```

### 7. What is URL routing in Django?
URL routing is the process of mapping a URL to a specific Django view. Django checks the URL patterns defined in `urls.py` and calls the corresponding view when a matching URL is requested.

```python
path("profile/", views.profile, name="profile")
```

### 8. What is `Promise.any()`?
`Promise.any()` is a JavaScript method that returns the result of the first Promise that successfully resolves. It ignores rejected Promises unless all Promises are rejected.

```javascript
Promise.any([promise1, promise2, promise3])
```

### 9. What is the difference between `render()` and `redirect()`?
`render()` returns an HTML template directly as the response, while `redirect()` sends the browser to another URL.

```python
return render(request, "home.html")
```

```python
return redirect("home")
```

### 10. What is `Meta` in Django forms?
`Meta` is an inner class in a Django ModelForm used to provide configuration for the form. It specifies which model the form is connected to and which model fields should be included.

```python
class UserForm(forms.ModelForm):
    class Meta:
        model = User
        fields = ["username", "email"]
```