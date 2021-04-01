FROM ubuntu:18.04
LABEL author="khaja ibrahim"
LABEL organization="QualityThought"
RUN apt update && apt-get install apache2 -y && mkdir spc
WORKDIR /spc
USER www-data
CMD ["whoami"]