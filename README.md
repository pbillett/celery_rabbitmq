
// https://docs.celeryproject.org/en/stable/getting-started/next-steps.html
// https://docs.celeryproject.org/en/stable/getting-started/first-steps-with-celery.html

# To create RabbitMQ instance:
If you’re using Ubuntu or Debian install RabbitMQ by executing this command:
sudo apt-get install rabbitmq-server

Or, if you want to run it on Docker execute this:
docker run -d -p 5672:5672 rabbitmq
(comme message queue on pourra aussi utiliser redis à la place)



# Install Celery:
pip install celery

#Starting the worker
The celery program can be used to start the worker (you need to run the worker in the directory above proj):
celery -A proj worker -l INFO


