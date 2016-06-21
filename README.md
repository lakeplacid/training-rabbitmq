# RabbitMQ training

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
- Use Vagrant with Ansible scripts from tools/ directory, it contains Ubuntu Xernial Xerus 64bit setup
  - In this scenario you will need [Vagrant](https://www.vagrantup.com) and [Ansible](https://www.ansible.com), latest versions
  - Ubuntu Xenial Xerus may throw network error during first  `vagrant up`. Please run `vagrant provision` then. VM may need some time to get up
- Import VirtualBox appliance during training, VM will be delivered on USB stick
  - In this scenario you will need [VirtualBox](https://www.virtualbox.org), latest version
