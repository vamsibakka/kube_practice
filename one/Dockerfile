FROM ubuntu:latest 
RUN apt update && apt install openjdk-17-jdk -y  && \
    apt install maven -y  && apt install git -y 
RUN https://github.com/vamsibakka/spring-petclinic.git
WORKDIR /spring-petclinic 
RUN mvn clean package
EXPOSE 8080
CMD [ "java","-jar","/target/*.jar" ]
