# building-a-blog-using-flask-and-angularjs

Source code of the application we are building on "Building a blog using Flask and AngularJS" tutorial series

See also https://github.com/Chitrank-Dixit/building-a-blog-using-flask-and-angularjs

## How to

* Clone this repository

    Run the following commands

        git clone xxxxx
        cd building-a-blog-using-flask-and-angularjs

* Create virtualenv and install requirements

    Run the following commands

        virtualenv -p python3 env
        source env/bin/activate
        pip install -r server/requirements.txt

    And install bower components

        cd client
        bower install

* Create sqlite database

    Create a sqlite database

        cd server
        python db_create.py

* Run server

    Start the flask server

        cd server
        python run.py

    Open a browser and navigate to `http://127.0.0.1:5000/api/v1/posts`, may see

        []

* Run client

    Start a http server

        cd client
        python -m http.server 8000

    Navigate to `http://127.0.0.1:8000`
