FROM ubuntu:latest 
RUN apt update && apt install openjdk-11-jdk -y  && \
    apt install wget -y && apt install maven -y  
RUN git clone https://github.com/spring-projects/spring-petclinic.git  &&  cd  ./spring-petclinic && mvn package
EXPOSE 8080
CMD [ "java","-jar","/target/*.jar" ]
