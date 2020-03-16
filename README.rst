=====
Polls
=====

This is from the "How to write reusable apps" Django tutorial.

https://docs.djangoproject.com/en/2.1/intro/reusable-apps/

Now that this app has been packaged independently,
(previously part of https://github.com/jshields/django-tutorial-mysite-project)
it has no way to run its own tests (no `manage.py`),
TODO provide a way to run tests: https://stackoverflow.com/questions/10897090/how-to-test-single-application-not-project-in-django

Polls is a simple Django app to conduct Web-based polls. For each
question, visitors can choose between a fixed number of answers.

TODO provide documentation in the "docs" directory.

Quick start
-----------

1. Add "polls" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'polls',
    ]

2. Include the polls URLconf in your project urls.py like this::

    path('polls/', include('polls.urls')),

3. Run `python manage.py migrate` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll.
