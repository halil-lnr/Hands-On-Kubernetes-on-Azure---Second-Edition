FROM openjdk:22-ea-29

CMD ["/usr/bin/java", "-jar", "/usr/share/myservice/myservice.jar"]

# Add Maven dependencies (not shaded into the artifact; Docker-cached)
ARG JAR_FILE
COPY target/${JAR_FILE} /usr/share/myservice/myservice.jar