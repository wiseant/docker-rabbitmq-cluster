FROM centos
MAINTAINER jayson jayson7710@gmail.com

RUN yum install -y wget unzip tar && 
    rpm -Uvh http://download.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-6.noarch.rpm &&
    yum install -y erlang &&
    rpm --import http://www.rabbitmq.com/rabbitmq-signing-key-public.asc &&
    yum install -y  http://www.rabbitmq.com/releases/rabbitmq-server/v3.6.2/rabbitmq-server-3.6.2-1.noarch.rpm

RUN /usr/sbin/rabbitmq-plugins enable rabbitmq_mqtt rabbitmq_stomp rabbitmq_management  rabbitmq_management_agent rabbitmq_management_visualiser rabbitmq_federation rabbitmq_federation_management sockjs

#CMD /usr/sbin/rabbitmq-server
