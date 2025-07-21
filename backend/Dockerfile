# Verwendet Java 17 JDK als Basis-Image
# Setzt das Arbeitsverzeichnis im Container auf /app
# Kopiert die .jar-Datei aus dem target-Ordner in den Container und nennt sie app.jar
# Öffnet Port 8080 für den Zugriff von außen
# Startet die Anwendung mit dem Befehl: java -jar app.jar

FROM eclipse-temurin:17-jdk-jammy

WORKDIR /app

COPY target/*.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]
