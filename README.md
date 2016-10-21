# How to use this image

The following environment variables are optional for docker-cloud:

-       `VIRTUAL_HOST=...`              (to use with docker-cloud automatic haproxy)
-       `USER_UID=...`                  (change www-data uid if variable exist)
-       `USER_GID=...`                  (change www-data gid if variable exist, default USER_UID)

Example stack file for docker-cloud
~~~
php-demo:
  environment:
    - VIRTUAL_HOST=php-demo.example.com
    - USER_UID=1001
    - USER_GID=1002
  image: 'hspotweb03/php-orgplan:latest'
~~~
