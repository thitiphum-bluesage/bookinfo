FROM ruby:2.7

WORKDIR /usr/src/app

COPY . .

RUN gem install webrick json net-http

EXPOSE 9080

ENV ENABLE_EXTERNAL_BOOK_SERVICE=true

CMD ["ruby", "details.rb", "9080"]