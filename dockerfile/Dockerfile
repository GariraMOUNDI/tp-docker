FROM java:8
WORKDIR /dockerfile
ADD tp-docker-1.0.0.jar tp-docker-1.0.0.jar
ENV env_username=tp_devops
ENV env_password=tp_devops
ENV env_url=127.0.0.1/tp_devops
EXPOSE 8080
CMD java -Ddatabase.url=$env_url -Ddatabase.username=$env_username -Ddatabase.password=$env_password -jar tp-docker-1.0.0.jar

