# What is it?

This project is a Rails 5 docker environment. The following tools are installed: 
* bundler
* Rails 5 release
* sqlidev
* NodeJS (it is required for some gems)

# Why should you use it?

First of all, it is helpful to run Rails and installs dependencies avoiding conflicts with other Rails projects. Also, it makes your local machine clean, so you don't need to install RVM or other stuff.

# How to use it?

There are two folders:
* mysql: when you want to create a Rails app on MySQL database
* sqllite: when you want to create a Rails app on SQLite database

After you clone the project, go to the folder of the database you want and read the README.md file present in the folder

# FAQ

=> **I already have a Rails project. How can I use this docker container?**
**A:** Pretty simple. Clone this docker container project and follow the steps:
* for mysql: copy the files .env, Dockerfile, docker-compose, entrypoint, Makefile, my.cnf and paste inside your Rails root path.  After that, type the command: ```make run```. Reminder yourself to edit your database.yml file using my example.database.yml as reference. If you have any questions, you can check [README.MD](./mysql/README.MD) inside the 'mysql' folder
* for sqlite:  copy the files Dockerfile, docker-compose, entrypoint, Makefile and pasta inside your Rails root path. After that, type the command: 'make run'. If you have any questions, you can check [README.MD](./mysql/README.MD) inside the 'mysql' folder

=> **I'm having problems to up the container or run the Rails project. What can I do ?**
**A:** create a [github issue](https://github.com/pierreabreup/docker-compose-for-rails5/issues) . I promise will answer as soon as possible
