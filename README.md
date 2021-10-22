# Django For Beginners Chapter 5: Blog

## Description
A very simple blog that allows CRUD through the superadmin account. This time there is a very simple frontend and we handle more routes leading to posts.

## New topic: Routing through html
Nothing groundbreakingly new. This is something I learned while studying Node with the MVC pattern but in Django things have different vocabularies and stuff.

To summarise how things are done in Django(as per my understanding so far):
1. The urlpatterns in urls.py in the main project first gets the request
2. Based on the pattern, the requests are routed to certain apps
3. The app takes the requst through their own urls.py file
4. The urlpattern in urls.py points to the Views(name seems misleading somehow as I come from nodejs)
5. The View uses a model(that interacts with the database) and html template to render a html template
6. The html template is returned and rendered on the client side

## Tests
Testing to see whether creating a post actually creates a post
Testing to see whether calling an existing routes gives a 200 response.
Testing to see whether calling a nonexistent routes gives a 404 response.
Testing to see whether the template used in the home.html template that is in the templates.
