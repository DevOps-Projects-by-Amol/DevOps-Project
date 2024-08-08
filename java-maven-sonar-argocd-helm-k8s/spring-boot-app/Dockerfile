FROM adoptopenjdk/openjdk11:alpine-jre

# Adjust the artifact path to match the working directory in the pipeline
ARG artifact=/workspace/java-maven-sonar-argocd-helm-k8s/spring-boot-app/target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

ENTRYPOINT ["java","-jar","app.jar"]
