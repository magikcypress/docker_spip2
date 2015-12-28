# Doker spip2

      $ sudo docker build -t dockers_spip2-0.0.1 .
      $ sudo docker run --name spip2-0.0.1 -v /etc/mysql -v /var/lib/mysql -v /var/www/spip -t -i dockers_spip2-0.0.1 bash
      $ sudo docker run --name spip2config --volumes-from spip2-0.0.1 -t -i dockers_spip2-0.0.1 bash