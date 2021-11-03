#
docker run --name my-nginx -v /usr/home/zwang/nginx/nginx.conf:/etc/nginx/nginx.conf:ro -d nginx -p 5000:80
docker run  -p 5000:80 --rm --name my-nginx -v /usr/home/zwang/nginx/conf.d:/etc/nginx/conf.d -d nginx


docker cp 2463b39c1786:/etc/nginx/nginx.conf ./nginx.conf