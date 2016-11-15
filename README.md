# Docker rabbitmq-dump-queue
Docker container for rabbitmq-dump-queue : Dumping rabbitmq queue easily

Build on https://github.com/dubek/rabbitmq-dump-queue

# Run example

docker run \
-e RABBITMQ_LOGIN=admin \
-e RABBITMQ_PWD=admin \
-e RABBITMQ_HOST=my.rabbit.server \
-e RABBITMQ_PORT=5672 \
-e QUEUE_NAME=payment.error \
-e MAX_MESSAGE=50 \
-v /tmp:/rabbitmq-dump-queue-result \
y0an:rabbitmq-dump-queue

