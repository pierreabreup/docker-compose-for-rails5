# How to use?

After you clone this project, follow the steps:
- open a terminal session in your terminal tool (Iterm, Terminal, Putty)
- go to folder where you've clone the project (Ex.: ```cd docker-compose-for-rails5```)
- go to folder 'mysql'
- type the command: ```make run```

This command will run the container and open a session inside the container. If all goes well, you will be in the path ```/usr/src/app```.   In this path, you can run commands like ```rails new my-rails-project```, ```gem install foo``` or anything else.

In Addition, make run will up database container and create a default database called 'rails5'. Feel free to use this database or create another.

It is worth noting that all database configuration inside docker-compose came from environemnt variable. So, if you have any questions, you can use the example.database.yml.

##### IMPORTANT!
when you run ```make run```in the first time, the docker image will be created. In the next times, docker compose will use the image.

# Extra tools

* If you want to up rails server, just type the command ```make rs``` in a new terminal session.
* If you want to up rails console, just tyoe the command ```make rc``` in a new terminal session.
