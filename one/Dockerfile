FROM ubuntu:latest 
RUN apt update && apt install openjdk-11-jdk -y  && \
    apt install wget -y && apt install maven -y  && install git -y 
RUN git clone https://github.com/spring-projects/spring-petclinic.git 
WORKDIR /spring-petclinic 
RUN mvn package
EXPOSE 8080
CMD [ "java","-jar","/target/*.jar" ]
