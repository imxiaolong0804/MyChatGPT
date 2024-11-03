docker run --name nginx \
-v /mydata/nginx/html:/usr/share/nginx/html \
-v /mydata/nginx/conf/nginx.conf:/etc/nginx/nginx.conf \
-v /mydata/nginx/conf/conf.d/default.conf:/etc/nginx/conf.d/default.conf \
-v /mydata/nginx/logs:/var/log/nginx\
--restart=always \
-p 80:80 -d nginx