FROM ruby:2.5.7
RUN gem install bundler
RUN gem install rails
RUN gem install rake
WORKDIR /app
COPY Gemfile Gemfile.lock ./
RUN bundle check || bundle install
COPY . /app
EXPOSE 3000