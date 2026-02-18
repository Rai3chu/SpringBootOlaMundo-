# Etapa 1: Usando a imagem base do OpenJDK
FROM openjdk:17-jdk-slim AS build

# Etapa 2: Definindo o diretório de trabalho no contêiner
WORKDIR /app

# Etapa 3: Copiando o arquivo JAR da pasta target para dentro do contêiner
COPY target/*.jar app.jar

# Etapa 4: Comando para rodar a aplicação Spring Boot
ENTRYPOINT ["java", "-jar", "/app/app.jar"]

# Etapa 5: Expondo a porta 8080 (padrão para Spring Boot)
EXPOSE 8080
