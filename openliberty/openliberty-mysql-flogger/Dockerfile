FROM sdaschner/open-liberty:javaee8-jdk11-b3
ENV SHARED_LIBS_DIR ${CONFIG_DIR}lib/global
RUN mkdir -p ${SHARED_LIBS_DIR}
ADD http://central.maven.org/maven2/mysql/mysql-connector-java/8.0.13/mysql-connector-java-8.0.13.jar ${INSTALL_DIR}lib
ADD http://central.maven.org/maven2/com/google/flogger/flogger/0.3.1/flogger-0.3.1.jar ${SHARED_LIBS_DIR}
ADD http://central.maven.org/maven2/com/google/flogger/flogger-system-backend/0.3.1/flogger-system-backend-0.3.1.jar ${SHARED_LIBS_DIR}
COPY mysql-driver.xml ${CONFIG_DIR}configDropins/defaults/