

  How  to sucessfully run the Restaurant Menu Web  application:

>  Purpose: this is an example of a Modern Data Driven-driven Web App constructed using Python, a Vagrant Virtual Machine, Flask framework and SQLAlchemy together         with SQLite.  The aim of the Restaurant Menu Web  application is to allow users to view restaurants and their respective menu items. Logged-in users will have the ability      to view, add, edit, and delete both menu items and restaurants which that he/ she created but NOT of other users.

> ACKNOWLEGEMENT : Special thanks to Udacity for using their materials from the course ud330 to do this project.

> Ensure you have the 'catalog' folder with you with all the following files and folders inside:

   1. lotsofmenus.py     2. database_setup.py     3. application.py     4. static folder	  5. templates folder

   6. fb_client_secrets.json  	 7. client_secrets.json  8. README.txt

   > Setup a Vagrant Virtual Machine using Git, Virtual Box and Vagrant software. Also ensure that Python version 2.7 is installed in your computer.

   > First, fork the fullstack-nanodegree-vm repository so that you have a version of your own within your Github account.

   > clone your fullstack-nanodegree-vm repository to your computer with the below command syntax in the Git bash terminal ( remember to run the Git bash program as             an administrator):

      git clone PASTE_PATH_TO_REPOSITORY_HERE fullstack

   - first type cd fullstack/vagrant, press enter

   - type vagrant up and press enter so as to power on the Vagrant Virtual Machine

   - type vagrant ssh and press enter to log into the  Vagrant Virtual Machine

   - next type cd /vagrant  and  press enter

   - type cd catalog, press enter

   - Now to sucessfully run the 'Restaurant Menu Web app', execute the following below steps in sequence :

     step 1: type python database_setup.py  and press enter  to initialize the database of the Restaurant Menu Web app.

     step 2: type python lotsofmenus.py and press enter to populate the Restaurant Menu Web app's database with restaurants and menu items.
     
     step 3: type  python application.py  and press enter to start the Flask application (application.py), then to view the  Restaurant Menu Web app, go to                                                   http://localhost:8000 on your web browser.

> User privileges on the Restaurant Menu Web app:

  a) For a Logged-in user: able to view, add, edit, and delete both menu items and restaurants which he or she created but NOT of other users.

  b) For a Visitor (a person who has not Logged-in ) : only be able to view both menu items and restaurants but CANNOT add, edit, or delete anything.

>  Viewing Restaurant Information with JSON  : go to following URLs

   a) http://localhost:8000/restaurant/JSON        - will show all restuarants.

   b) http://localhost:8000/<int:restaurant_id>/menu/JSON      - will show a specific restaurant and all its menu items. Like  http://localhost:8000/restaurant/1/menu/JSON

   c) http://localhost:8000/restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON    - will show a specific restaurant and a specific menu item of that particular restaurant.                                                                                                                                         Like http://localhost:8000/restaurant/1/menu/2/JSON

