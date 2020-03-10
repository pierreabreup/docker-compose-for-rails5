FROM ruby:2.5-alpine

RUN apk add --no-cache bash
RUN apk add --update \
  build-base \
  ruby-nokogiri \
  nodejs \
  libxml2-dev \
  libxslt-dev \
  sqlite-dev \
  && rm -rf /var/cache/apk/*

EXPOSE 3000

WORKDIR /usr/src/app

RUN gem install rails

COPY ./entrypoint.sh /etc/entrypoint.sh
RUN chmod +x /etc/entrypoint.sh
CMD ["/bin/sh"]
ENTRYPOINT ["/etc/entrypoint.sh"]
