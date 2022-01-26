**[commands]()**
- C1 - `python manage.py migrate`
- C2 - `python manage.py makemigratios`


**Migration :** it means storing the change I wanna bring on db tables.

## CREATING A MODEL:
- open models.py of your app where you wanna add a model.
- make a class named <anything related to the model>. And inherit `models.Model` in this class.
- run C2  command
- run C1
    - this command will store migrations in migrations folder of the app.
    - this command does not write the change in db
- run C2 again this will write changes in database
- To view your tables on admin panel register your models.

## Registering a model.
- go to`admin.py` of desired app
- write `from . models import product` in it .
- Write `admin.site.register(<model name>)`
- 
- 
- 


**Note :** First `makemigrations` then 
`migrate`
