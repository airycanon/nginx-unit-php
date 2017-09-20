# NGINX Unit with PHP

NGINX Unit is a dynamic web application server, designed to run applications in multiple languages. 

# Documentation
See http://unit.nginx.org/docs-nginx-unit.html.

# Run
```
git clone https://github.com/airycanon/nginx-unit-php.git
cd nginx-unit-php
$ docker run -v `pwd`/applications:/applications -v `pwd`/run:/var/run:rw -p 8300:8300
```

# Test
```
cd nginx-unit-php
sudo curl -X PUT -d @./json/test.json --unix-socket ./run/control.unit.sock http://localhost/ 

```
See http:://localhost:8300


