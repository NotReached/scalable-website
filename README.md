# A Scalable Website using AWS and ECS
<p>
<b> Run this first, probably getting 172.12.0.2</b><p>
`docker run -d -v /www:/www -p 80:80 dd/tengine:1.0`<p>
<b> Run this second, probably getting 172.12.0.3</b><p>
`docker run -d -v /www:/www -p 9000:9000 dd/php:1.0`<p>
<b> Run this last, probably getting 172.17.0.4</b><p>
`docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=test mariadb`<p>
<p>
<p>
<b> The IP's may be different and I'll probably end up changing the method of the connection but this worked.</b><p>
