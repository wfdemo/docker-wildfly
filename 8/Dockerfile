FROM sewatech/wildfly:8
MAINTAINER Alexis Hassler <alexis@sewatech.org>

RUN mv /wildfly-$WILDFLY_VERSION /wildfly &&\
    /wildfly/bin/add-user.sh --silent admin passw0rd!

COPY desc.txt /
COPY standalone.conf /wildfly/bin/

WORKDIR /wildfly
EXPOSE 8080 9990

ENTRYPOINT []
CMD ["/wildfly/bin/standalone.sh"]
