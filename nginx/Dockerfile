FROM tutum/nginx
RUN rm /etc/nginx/sites-enabled/default
ADD sites-enabled/ /etc/nginx/sites-enabled
RUN apt-get update
RUN apt-get -y install apache2-utils
RUN mkdir /etc/nginx/passwd
RUN htpasswd -c -b /etc/nginx/passwd/kibana.passwd steven StevenPassword000