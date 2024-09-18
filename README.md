# we have to install Two python packages inorder to connect mysql to ur django project 
1. pip install pymysql 
2. pip install mysql-connector-python

## Now Configuring with in the settings.py tfile of your project 
import pymysql 
pymysql.version_info=(1,4,6,"final",0) 
pymysql.install_as_MySQLdb() 

## now after this scroll down to database section 
      DATABASES = { 
      'default': { 
      'ENGINE': 'django.db.backends.mysql', 
      'NAME': 'name of the database u have created', 
      'USER':'root', 
      'PASSWORD':'root', 
      'HOST':'localhost', 
      'PORT':3306, 
       }
      }
