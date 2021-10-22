# Django For Beginners Chapter 5~: Blog

## Description
A very simple blog that allows CRUD through forms. This time there is a very simple frontend and we handle more routes leading to posts.

## New topic 1(chapter 5): Routing through html
Nothing groundbreakingly new. This is something I learned while studying Node with the MVC pattern but in Django things have different vocabularies and stuff.

To summarise how things are done in Django(as per my understanding so far):
1. The urlpatterns in urls.py in the main project first gets the request
2. Based on the pattern, the requests are routed to certain apps
3. The app takes the requst through their own urls.py file
4. The urlpattern in urls.py points to the Views(name seems misleading somehow as I come from nodejs)
5. The View uses a model(that interacts with the database) and html template to render a html template
6. The html template is returned and rendered on the client side

## New topic 2(chapter 6): Forms
No more making stuff through superadmin. Now we have forms. I don't like writing html/css but oh well.
Was able to make a simple CRUD with forms. I wonder when I can actually hook up a real database instead of an sqlite3 db. I'm also beginning to see a pattern on how to write and implement new things in Django:
1. Make a html page or edit existing one that will send the request
2. Create a view that will handle the request in Views
3. Add a url to Urls that will connect the request with a url to the Views

## New topic 3(chapter 7): User
Good old user authentication. Django really abstracts away a lot of the stuff needed for this stuff so it is really really convenient. I'm kinda glad I was forced to do all of this manually by nodejs because now I appreciate this stuff so much more.

## Tests
* Testing to see whether creating a post actually creates a post
* Testing to see whether calling an existing routes gives a 200 response.
* Testing to see whether calling a nonexistent routes gives a 404 response.
* Testing to see whether the template used in the home.html template that is in the templates.
* Testing to see whether create, update, delete views work
