# What's this?
- This is a Web application template with Nginx and Gunicorn.

# Constitution
- Web Server
  - nginx
- WSGI Server(AP server)
  - Gunicorn
- Web Application Framework
  - Django
    - This project uses WSGI, so you can use other framework which base on WSGI.
    - This project does not contain unique settings for Django.
- The Web server and WSGI Server will run in Docker container.
- UNIX domain socket is used in communications between the Web server and WSGI Server.

# Prerequisite
- You can use `pip` and `docker` command.
- The port `8000` can be used.

# How to use
- Install python package.
  - `$ pip install -r requirements.txt`
- Start servers.
  - `$ docker-compose up -d`
  - Then you can access `localhost:8000` in your browser and the default page for Django will be shown.
  
# Details
- [My article at Qiita(In Japanese)](https://qiita.com/str416yb/items/7324b99b9f05b9089b80)
