FROM ubuntu:latest 
RUN apt install update && apt install openjdk-11-jdk && \
    apt install wget -y && apt install maven -y  
RUN wget https://github.com/spring-projects/spring-petclinic.git 
WORKDIR   /spring-petclinic
RUN  mvn package 
EXPOSE 8080
CMD [ "java","-jar","/target/*.jar" ]
