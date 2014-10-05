Restful Objects Vagrant
=======================

This project is a simple Vagrant setup file to bootsrap easily a VM with the [Restful Objects for Ruby framework](http://github.com/vizcay/RestfulObjectsRuby) installed.

### Instructions

1. Install Vagrant for your operating system (Linux, Mac & Windows supported):

  [Vagrant Downloads](https://www.vagrantup.com/downloads.html)

2. Clone this project:

  ```shell
  git clone https://github.com/vizcay/restful_objects_vagrant
  cd restful_objects_vagrant
  ```

3. Vagrant up the VM:

  ```shell
  vagrant up
  ```

  This will take a few minutes, but after the VM will be provisioned with:
  - Ubuntu 14.04 32bits
  - Ruby 1.9.3
  - RubyGems & Bundler
  - Restulf Objects for Ruby (latest version)

4. To start a server create some restful_object_script in your project root, and to start the framework execute:

  ```shell
  vagrant ssh -c "cd /vagrant && restful_server restful_object_script.rb"
  ```

  Now you will be able to connect to the restful server in your host by opening http://localhost:4567

