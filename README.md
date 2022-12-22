# django-tutorial

# Polls

Polls is a Django app to conduct web-based polls. For each question,
visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

## Quick start

1. Add "polls" to your INSTALLED_APPS setting like this:

    ```python
    INSTALLED_APPS = [
        ...
        'polls',
    ]
    ```

2. Include the polls URLconf in your project urls.py like this:

    ```python
    path('polls/', include('polls.urls')),
    ```

3. Run `python manage.py migrate` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/ to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll.


# When starting a new project:
```zsh
# initialise project
poetry new django-tutorial

# delete tests directory
rm -R tests/

# create repo
git init

# create .gitignore
echo .venv/ > .gitignore

# create .tool_versions
asdf local python latest

# create venv
echo "layout poetry" > .envrc
direnv allow

# install packages
poetry add django

# create project
poetry run django-admin startproject django_tutorial .

# start development server
# python manage.py runserver

# build project
poetry build
```
