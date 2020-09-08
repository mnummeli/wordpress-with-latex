FROM wordpress:latest

RUN \
  apt-get update && \
  apt-get install -y nano wget unzip && \
  cd /var/www/html/wp-content/plugins && \
  wget https://downloads.wordpress.org/plugin/wp-quicklatex.3.8.6.zip && \
  unzip wp-quicklatex.3.8.6.zip && \
  rm wp-quicklatex.3.8.6.zip