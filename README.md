# et2598-raer18-workshop2
In this assignment we have to implement a simple web service. For that we have to create servers namely,

1.devA 

2.devB

3.devC

4.devhaproxy and

5.Bastion.

Through ansible playbook it installs nginx and php-fpm in servers devA, devB and devC to make the work more efficient.

Then it setups nginx.conf file at etc/nginx and remove "default" site at etc/nginx/sites-enabled.

Now it setups nginx.conf file at etc/nginx/sites-available.Then it links default etc/nginx/sites-available to etc/nginx/sites-enable.

Then it setups index.php file at root var/www/html.

Through ansible playbook it installs haproxy load balancer to distribute the load between the servers.

Then it pushes haproxy configuration file haproxy.cfg.j2 to etc/haproxy/haproxy.cfg.

Now it setups default starting flag to 1 in etc/default/haproxy.

And the bastion acts as jump host and provides secuity.
