# What is it?

This project is a rails 5 docker environemtn. The following tools aready installed: bundler, last rails 5 release, sqlidev, nodejs (it is required for some gems)

# Why use it?

First of all, it is helpful to run rails and installs dependencies avoiding conflicts with other rails projects. The second reason, it is to make your local machine clean, you don't need to install RVM or other stuff.

# How to use?

After you clone this project, follow the steps:
- open a terminal session in your terminal tool (Iterm, Terminal, Putty)
- got to folder where you've clone the project (Ex.: ```cd docker-compose-for-rails5```)
- type the command: ```make run```

This command will run the container and open a session inside the container. If all goes well, you will be in the path ```/usr/src/app```.   In this path, you can run commands like ```rails new my-rails-project```, ```gem install foo``` or anything else.

##### IMPORTANT!
when you run ```make run```in the first time, the docker image will be created. In the next times, docker compose will use the image.

# Extra tools

* If you want to up rails server, just type the command ```make rs``` in a new terminal session.
* If you want to up rails console, just tyoe the command ```make rc``` in a new terminal session.
