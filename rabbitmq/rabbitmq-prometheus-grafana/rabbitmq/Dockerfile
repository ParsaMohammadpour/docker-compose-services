FROM rabbitmq:3-management

RUN apt-get update && apt-get install -y wget
RUN rabbitmq-plugins enable rabbitmq_tracing
RUN rabbitmq-plugins enable rabbitmq_management
RUN rabbitmq-plugins enable --offline rabbitmq_management

EXPOSE 5672 15672 15671

CMD ["rabbitmq-server"]