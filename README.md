# twitter-clone-django
Twitter Clone made using Django


Description : A basic clone of twitter

DB used:  default db.sqlite3


Pages and web Hooks

## admin:
    Admin page

## accounts
    Accounts page
    Basic Accounts functionality such as Sign Up, Login, Logout, etc
    Views/Web Hooks
        signup/  :: signup for the application
        login/   :: login functinoality
        logout/   :: Logout functinoality
        all/    :: get all users of application
        ajax/change-follow-status/ :: toggle status of follower/following
        ajax/check-follow-status/ :: check status of follower/following
    
    Models/DB
        Django default user Model used

## tweets
    Tweets Page
    All functionality regarding tweets
    Views/Web Hooks
        new/ ::create a new tweet
        my-tweets/<username> :: show all the users' tweet
        delete/<int:pk> :: delete the marked tweet
        home-tweets/<int:pk> :: go for specific tweet details

    Models/DB
        Tweets
        fields:  user(from accounts), Tweet content, created at(auto populaated)





Instruction for starting
##requirment
Python version 3.6+

1. once directed to the main project, use python -m pip install pipenv --upgrade
2. then run pipenv shell to run the env,
3. use pipenv to create and install virtual env and requirments.txt using pipenv install -r requirements.txt 
4. do the migrations using ./mamage.py makemigrations [please note that you should be in the directory with manage.py file, incase we see some error for modules not found, please install them using pipenv <moduleName>]
5. do the migrations using ./mamage.py migrate
6. Run ./manage.py createsuperuser [to create a super admin for admin page]
7. run ./manage.py runserver.



--Vivek Singh