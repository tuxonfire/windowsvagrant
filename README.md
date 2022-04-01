### Windows2019 using Vagrant and some basic Ansible playbooks 

Install Vagrant. Instrunctions [here](https://www.vagrantup.com/docs/installation).

Clone the repo:

```
git clone git@github.com:tuxonfire/windowsvagrant.git
```
cd windowsvagrant/

~~~
vagrant up
~~~

Details about the script can be read below link, and can be used to set up the basics on WIndows 2019 (i think is free for 90 days). This script sets up both HTTP and HTTPS listeners with a self-signed certificate and enables the 'Basic' authentication option on the service.

https://docs.ansible.com/ansible/latest/user_guide/windows_setup.html#winrm-setup

Use remmina to connect (RDP/SSH)
![Screenshot from 2022-03-31 20-26-19](https://user-images.githubusercontent.com/7489885/161183158-91b99a1d-5ddb-4fd0-9dc8-a6b4f5363ef4.png)
