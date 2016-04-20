FROM maven

#install git
RUN apt-get -y update && apt-get install -y git

# Clone the project
RUN git clone https://github.com/abdulbasitkay/guestbook

# run the application
#RUN cp ./guestbook/* /
RUN cd guestbook &&  mvn clean package
RUN cat ./guestbook/pom.xml
CMD ["mvn" , "spring-boot:run"]