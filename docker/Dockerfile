FROM ubuntu

RUN apt-get update && apt-get install -y \
  supervisor \
  vim \
  curl

ADD supervisord.conf /etc/supervisor/supervisord.conf

CMD ["supervisord", "-c", "/etc/supervisor/supervisord.conf", "-n"]

#CMD tail -f /dev/null
