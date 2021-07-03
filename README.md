# dockerthing
> Dcoker tips and review


__manip:__
- docker run --name web -dt nginx 
- docker exec web mkdir /var/www/

__By default /usr/share/nginx/html/ is home of index.html but we can change the default conf as follows__

- docker cp .\default.conf web:/etc/nginx/conf.d 
- docker cp .\jof\ web:/var/www
- docker stop web
- docker run --name web01 -dt -p 8080:80 web-base

>what should run: docker run -dt -name web01 -p 8080:80 web-im ==> 8080 from host 80 fom container
