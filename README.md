# django-tutorial

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

# creating the project
poetry run django-admin startproject django_tutorial .
```
