# What is it?

This project is a rails 5 docker environemtn. The following tools aready installed: bundler, last rails 5 release, sqlidev, nodejs (it is required for some gems)

# Why use it?

First of all, it is helpful to run rails and installs dependencies avoiding conflicts with other rails projects. The second reason, it is to make your local machine clean, you don't need to install RVM or other stuff.

# How to use?

There two folder:
* mysql: when you want to create a rails app on mysql database
* sqllite: when you want to create a rails app on sqlite database

After you clone the project, go to the folder of the database you want and read README.md file present in the folder

# FAQ

=> **I already have a rails project. How can I use this docker container?**
**A:** Pretty simple. Clone this docker container project and follow the steps:
* for mysql: copy the files .env, Dockerfile, docker-compose, entrypoint, Makefile, my.cnf and paste inside your rails root path.  After that, type the command: ```make run```. Reminder yourself to edit your database.yml file using my example.database.yml as reference. If you have any questions, you can check [README.MD](./mysql/README.MD) inside the 'mysql' folder
* for sqlite:  copy the files Dockerfile, docker-compose, entrypoint, Makefile and pasta inside your rails root path. After that, type the command: 'make run'. If you have any questions, you can check [README.MD](./mysql/README.MD) inside the 'mysql' folder

=> **I'm having problems to up the container or run rails project. What can I do ?**
**A:** create a [github issue](https://github.com/pierreabreup/docker-compose-for-rails5/issues) . I promise will answer as soon as possible
