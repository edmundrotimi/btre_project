# Setting Up 

1. Requirements:

    ``` setup 
    
    django
    Pillow
    psycopg
    
    ```
2. Database:

    ``` setup 
    
    'NAME': '<db anme>',
    'USER' : '<db user>',
    'PASSWORD' : '<db password>',
    'HOST' : '<db host>',
    
    ```
       
3. Apply the migrations, create a superuser, and add the fixtures to the DB:

    ``` setup 
    
    $ python manage.py migrate
    $ python manage.py collectstatic
    $ python manage.py createsuperuser
    
    ```
    
4. Add your email setup to *settings.py* file:

    ```python
    EMAIL_HOST = '<host here>'
    EMAIL_HOST_USER = '<username here>' # this is exactly the value 'apikey'
    EMAIL_HOST_PASSWORD = '<pass here>'
    EMAIL_PORT = '<port here>'
    EMAIL_USE_TLS = True
    ```
