# HELK script: HELK Elasticsearch Dockerfile
# HELK build Stage: Alpha
# HELK ELK version: 6.3.2
# Author: Roberto Rodriguez (@Cyb3rWard0g)
# License: GPL-3.0

# References: 
# https://cyberwardog.blogspot.com/2017/02/setting-up-pentesting-i-mean-threat_98.html

FROM docker.elastic.co/elasticsearch/elasticsearch:6.3.2
LABEL maintainer="Roberto Rodriguez @Cyb3rWard0g"
LABEL description="Dockerfile base for the HELK Elasticsearch."

RUN /usr/share/elasticsearch/bin/elasticsearch-keystore create
RUN printf "elasticpassword" | /usr/share/elasticsearch/bin/elasticsearch-keystore add "bootstrap.password"