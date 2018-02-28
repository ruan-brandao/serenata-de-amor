FROM fluent/fluentd:v0.12.42

COPY fluent.conf /fluentd/etc

RUN apk add --no-cache --virtual build-base \
  && apk add --no-cache --virtual ruby-dev
RUN gem install fluent-plugin-elasticsearch --no-rdoc --no-ri --version 2.7.0
