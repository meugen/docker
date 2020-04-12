# Sample java application
FROM openjdk:14-alpine
LABEL Author="Yevgeniy Malyshev"

COPY Sample.java /sources/
WORKDIR /sources
RUN javac Sample.java && rm Sample.java

CMD java Sample