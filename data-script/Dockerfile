FROM alpine

RUN apk update
RUN apk add mysql-client

COPY import.sh /opt
COPY mydatabase.sql /opt
WORKDIR /opt
RUN chmod +x import.sh
CMD ["/bin/sh", "import.sh"]
