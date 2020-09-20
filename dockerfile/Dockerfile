FROM java:8
WORKDIR /dockerfile
ADD tp-docker-1.0.0.jar tp-docker-1.0.0.jar
ARG username=admin
ARG password=123456
ARG url=127.0.0.1/tp_devops
ENV env_username=$username
ENV env_password=$password
ENV env_url=$url
EXPOSE 8080
CMD java -Ddatabase.url=$env_url -Ddatabase.username=$env_username -Ddatabase.password=$env_password -jar tp-docker-1.0.0.jar

