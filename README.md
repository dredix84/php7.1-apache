# php7.1-apache #
This is a container contains Apache2.2 and PHP 7.1 with a few additional extensions installed. The reason for creating this container was to give a a good starting base for developing my CakePHP 3 application, however, you create run other PHP scripts or frameworks if needed..

Additional Extentions
___
- intl
- mcrypt
- mbstring
- pdo_mysql
- zip
- calendar

## Runnning this image

**Step 1** (build docker image)
```bash
docker build -t php7apache .
```
**Step 2** (Run docker container)
```bash
docker run -d -v .:/var/www/html -p 8080:80 --name mywebserver php7apache
```

The files from you current directory you are executing the above command will be in the root of `/var/www/html`.


Author
----
Andre Dixon