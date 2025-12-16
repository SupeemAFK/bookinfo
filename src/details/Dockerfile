FROM ruby:2.7

WORKDIR /app

COPY Gemfile .

RUN bundle install

COPY . .

EXPOSE 9080

CMD ["ruby", "details.rb", "9080"]
