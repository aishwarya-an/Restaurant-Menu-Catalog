# Restaurant Menu App


## Overview

This project aims to make use of the Flask framework where restaurants are listed with their menus. Using third-party authentication by way of Google+, logged-in users can: create, update, and delete their own restaurants and corresponding menus.

## Configuration Instructions

This project requires:

1. Python Libraries: requests, oauth2client, and httplib2
2. Python 2.7
3. Postgresql
4. SQLAlchemy
5. Flask 0.12.1

## Installation

* Assuming you have downloaded the application code, navigate to the directory
where database_setup.py lives and run: `python database_setup.py`.
* This will
set up the database. Once the database is created you can run
`python lotsofmenus.py` to populate the database with useful prearranged
content.

* You you are using Vagrant then, run `vagrant up` followed by
`vagrant ssh`. If you do not use Vagrant, then install SQLAlchemy
from the following link: http://www.sqlalchemy.org.

## Operating Instructions

JSON endpoints are available and they can be accessed by simply visiting the
following URLs:

1. `localhost:5000/restaurant/<int:restaurant_id>/menu/JSON`  - to find a restaurant menu)
2. `localhost:5000/restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON` - to find a menu item)
3. `localhost:5000/restaurant/JSON` - to find the restaurants)

## How to Run Code

1. Run `python project.py` in the appropriate path on the command line.
2. Go to your web browser and input: `http://localhost:5000`.
3. In the top-right of the page for the app, click "Log in".

* You you are using Vagrant then, run `vagrant up` followed by
`vagrant ssh`. Then go to the catalog directory by running  
`cd /vagrant/catalog` and to execute the application, run `python project.py`.
