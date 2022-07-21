FROM ruby:3.1.0

RUN mkdir /api
WORKDIR /api
COPY Gemfile /api/Gemfile
COPY Gemfile.lock /api/Gemfile.lock
RUN bundle install
COPY . .

CMD ["rails", "server", "-b", "0.0.0.0"]
