# dj-shop
Online Shop made by Django Python Framework


### RabbitMQ in a Docker
```
 docker pull rabbitmq:3.13.1-management
 docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.13.1-management
```

-  Open http://127.0.0.1:15672/ in your browser.
-  Credentials guest/guest

###  Running a Celery worker
- Open another shell and start a Celery worker from your project directory, using the following command:
```
 celery -A myshop worker -l info
```

-  Open http://127.0.0.1:15672/ in your browser to access the RabbitMQ management UI.

