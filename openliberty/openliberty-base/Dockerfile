FROM openjdk:11
LABEL maintainer="Víctor Cabrera <asniaire@gmail.com>"
ENV RELEASE=2018-11-21_0300
ENV VERSION=18.0.0.4
RUN curl https://public.dhe.ibm.com/ibmdl/export/pub/software/openliberty/runtime/release/${RELEASE}/openliberty-${VERSION}.zip -L -o openliberty.zip && unzip openliberty.zip -d /opt && rm openliberty.zip

ENV INSTALL_DIR=/opt/wlp/
ENV CONFIG_DIR=/opt/wlp/usr/servers/defaultServer/
ENV DEPLOYMENT_DIR=/opt/wlp/usr/servers/defaultServer/dropins/

CMD ["/opt/wlp/bin/server", "run", "defaultServer"]