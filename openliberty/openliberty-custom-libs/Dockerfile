FROM asniaire/openliberty:mysql5.7
LABEL maintainer="Víctor Cabrera <asniaire@gmail.com>"

ENV SHARED_LIBS_DIR ${CONFIG_DIR}lib/global

RUN mkdir -p ${SHARED_LIBS_DIR}

ADD http://central.maven.org/maven2/com/google/flogger/flogger/0.3.1/flogger-0.3.1.jar ${SHARED_LIBS_DIR}
ADD http://central.maven.org/maven2/com/google/flogger/flogger-system-backend/0.3.1/flogger-system-backend-0.3.1.jar ${SHARED_LIBS_DIR}

ADD http://central.maven.org/maven2/org/flywaydb/flyway-core/5.2.4/flyway-core-5.2.4.jar ${SHARED_LIBS_DIR}

ADD http://central.maven.org/maven2/net/wasdev/wlp/tracer/liberty-opentracing-zipkintracer/1.2/liberty-opentracing-zipkintracer-1.2-sample.zip .
RUN unzip liberty-opentracing-zipkintracer-1.2-sample.zip -d $INSTALL_DIR/usr/ && rm -rf liberty-opentracing-zipkintracer-1.2-sample.zip
