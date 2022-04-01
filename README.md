#Windows2019

~~~
vagrant up
~~~

Details about each component can be read below link, but the script ConfigureRemotingForAnsible.ps1 can be used to set up the basics. This script sets up both HTTP and HTTPS listeners with a self-signed certificate and enables the 'Basic' authentication option on the service.

https://docs.ansible.com/ansible/latest/user_guide/windows_setup.html#winrm-setup
