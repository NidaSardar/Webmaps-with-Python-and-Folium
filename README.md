# Portfolio-with-Python-and-Flask

08-08-2020 || Nida Sardar

---

## Description.

Portfolio is kind of website which shows the information of equivalent to resume.

Flask is a python framework having templates and functions for you to create pyhton website.

Heroku is service that allows to deploy python applications on their cloud. They provide free deployment, domain name for website and zero maintenance and administration work of servers.

This is basic application which is about how you can creat basic portfolio/website using flask and make it live on Herouku server. 

The steps focuses how you can create application using Flask and deploy it on live server!!!

--------

## Files Description.
1. script1.py 
2. requirements.txt
3. Procfile
4. runtime.txt
5. /templates/about.html
6. /templates/home.html
7. /templates/layout.html
8.  /static/css/main.css


## Steps to deploy python website on Herouku Server.

1. Create Heroku account.
2. Install Heroku tool belt. The tool allows Heroku server to communicate through CLI.
3. To login in Heroku Website, run following command in CLI.
    
        heroku login
4. After running command. provide credentials.
5. Create app by running following command.
    
        heroku create app_name
6. To list all apps of Heroku, run
    
        heroku apps

7. Create three files in same directory.Descriptio of files are:

    - requirements.txt : it contains list of dependencies that you want Heroku to install.
    - Procfile : without extension file tells Heroku what web server to use to run application.
    - runtime.txt : Heroku needs runtime.txt file to know which python version needs to be install for application.Check currently available python runtime on Heroku's website before creating this file.
8. Run following commands:

        git init
        git add .
        git commit -m "First commit"
        heroku git : remote --app app_name
        git push heroku master

9. To see your live applicatio, run

        heroku open.
    It will redirect you to your live webiste.
10. To check the information, run

        heroku info