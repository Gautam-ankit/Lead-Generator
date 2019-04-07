# Lead-Generator
A Full stack project developed using Django and React, Redux.

Create a Project folder/ open in VS code/ open terminal

First check out the verion of Python Installed as well as install virtual enviornment.

~ pip install pipenv

then run command pipenv shell for entering and working in the virtual environment. Now a pip file is created down on the project folder.

Go for installing some more stuff

~pipenv install django
~pipenv install djangorestframework
~pipenv install django-rest-knox

a pipfile.lock file is created in addition to some changes in packages in pipfile.

# Now we will create our project using command

~django-admin startproject leadmanager

goto the leadmanager folder using 

~cd leadmanager command

# Now select the correct environment for VS code 
// press ctrl + shift + p and start typing python and select python interpreter then select option with your filename.

# creating Django App

~ python manage.py startapp leads

# whenever we create a Django app we need to add that stuff to the setting.py file
i.e. INSTALLED_APPS =[
  'rest_framework'
  'leads'
]

# creating models by creating class in models.py

# After creating a model we need to migrate that
~ python manage.py makemigrations
(fetches the structure of table according to the model)

~python manage.py migrate
(creates the table for required structure)

# Creating serializers which converts models into JSON object by creating serializers.py

# bringing models into the picture by creating api.py

within this file we will create queryset to access the data and permissions and opt the serializer class

# creating URLs
by default Django comes with an admin area but this time we don't want any superuser and we will include a seperate file for that, we will create urls in the lead folder using routers  and sent it here.

created urls.py in leads folder and redirected it to root urls.py using default router.

---------------------END----------------------



