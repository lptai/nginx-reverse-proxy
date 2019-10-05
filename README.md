
# How to run?

- Install nginx
- Start nginx with `sudo nginx -p $(pwd) -c nginx.conf`
- By default, it listens to port 80 (that's why you need sudo for that)
- All other paths will be forwarded to `localhost:3000`


`nginx -v`

> sudo nginx -p `pwd`/ -c nginx.conf

> sudo kill -QUIT `cat nginx.pid`

reloading

> sudo kill -HUP `cat nginx.pid`


> ps aux | grep nginx

# generate ssl key
`sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout nginx-selfsigned.key -out nginx-selfsigned.crt`