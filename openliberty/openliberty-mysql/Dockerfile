FROM sdaschner/open-liberty:javaee8-jdk11-b3
LABEL maintainer="Víctor Cabrera <asniaire@gmail.com>"

ADD http://central.maven.org/maven2/mysql/mysql-connector-java/8.0.13/mysql-connector-java-8.0.13.jar ${INSTALL_DIR}lib
COPY mysql-driver.xml ${CONFIG_DIR}configDropins/defaults/