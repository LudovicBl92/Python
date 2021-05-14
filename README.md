# Python

This playbook has been validated on systems Ubuntu 18:04 and CentOS 7

I want to install an environment python for developers by following the url: https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server-fr

The playbook run_python.yml is a basicaly playbook it permit to call the role Python

In the role Python there is 3 tasks:
- install_python.yml (update/upgrade/install Python and other packages
- Create_env.yml (allow the developer to develop in his environment)
- main.yml (import the tasks)

There is in the directory Python/vars the main.yml file who contain some variables

Finaly, run the playbook run_python.yml and when the playbook is finished:
- go to your host then your directory which contain your python environment
- run the command source First_environment/bin/activate
- run the command python hello.py == it will return your Hello, World!
