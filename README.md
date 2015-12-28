# Doker spip2

Create container for [SPIP2](http://www.spip.net) 

Container use debian:wheezy + SPIP 2.1.28

      $ sudo docker build -t dockers_spip2-0.0.1 .
      $ sudo docker run --name spip2-0.0.1 -v /etc/mysql -v /var/lib/mysql -v /var/www/spip -t -i dockers_spip2-0.0.1 bash
      $ sudo docker run --name spip2config --volumes-from spip2-0.0.1 -t -i dockers_spip2-0.0.1 bash

## Version 0.0.1

- Install Apache
- Install Mysql
- Install SPIP2
- Test Build
- Add entrypoint
- Add bash script 
- Add apache config
- Add volume