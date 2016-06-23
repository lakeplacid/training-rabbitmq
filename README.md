# RabbitMQ training

## Project

During workshop we will implement small feed-style app. System will be implemented as two separated apps, communicating by messages via RabbitMQ:

- HTTP API based on Slim microframework for:
  - publishing message
  - displaying user stream
  - displaying user followers
- backend workers, responsible for background data processing

### Project details

Non-technical details:

- User may follow other users
- User may publish a message with single string
- Message publishing must be fast, because single user may be followed by 1.000.000 of other users

Technical details:
  
- User have pre-generated stream of messages written by observed users
- For workshop purposes memory is sufficient to store user data (observed users)
- For workshop pupposes files are sufficient to store pre-generated stream data (one file per user) 

## Requirements

During the training you will need your own device with some software installed:

- PHP 5.6.x or 7.0.x with modules:
  - ext-bcmath
  - ext-mbstring
- composer
- [RabbitMQ server](https://www.rabbitmq.com/download.html)
- git

And last but not least... willingness to learn.

### How to prepare environment?

You can choose one of following methods:

- Prepare your device on your own
- Use Vagrant with Ansible scripts from tools/ directory, it contains Ubuntu Xenial Xerus 64bit setup
  - In this scenario you will need [Vagrant](https://www.vagrantup.com) and [Ansible](https://www.ansible.com), latest versions
  - Ubuntu Xenial Xerus may throw network error during first  `vagrant up`. Please run `vagrant provision` then. VM may need some time to get up
- Import VirtualBox appliance during training, VM will be delivered on USB stick
  - In this scenario you will need [VirtualBox](https://www.virtualbox.org), latest version
