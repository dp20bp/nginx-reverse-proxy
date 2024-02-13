# Notes

> docker build . -t nginx-base-reverse-proxy:latest

> docker run -d --name my-nginx-base-reverse-proxy -p 80:80 nginx-base-reverse-proxy:latest

# --> Open Browser
URL http://localhost:80
URL http://localhost/sample

## - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
[Test]
> docker cp ./nginx.conf my-nginx-base-reverse-proxy:/etc/nginx/ && docker cp ./default.conf my-nginx-base-reverse-proxy:/etc/nginx/conf.d/ && docker exec my-nginx-base-reverse-proxy nginx -t && docker exec my-nginx-base-reverse-proxy nginx -s reload
## - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

