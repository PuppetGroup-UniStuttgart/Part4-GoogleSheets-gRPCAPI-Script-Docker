FROM maven:3.3-jdk-8

# Get sources
RUN git clone --recursive https://github.com/shruthikuki/UniStuttgart-PuppetGroup-gRPCGoogleSheets.git
WORKDIR /UniStuttgart-PuppetGroup-gRPCGoogleSheets

# Run maven
RUN mvn clean package
RUN ls target

COPY config.properties /

WORKDIR /

CMD sleep 5s; java -cp /UniStuttgart-PuppetGroup-gRPCGoogleSheets/target/gRPCGoogleSheets-0.0.1-SNAPSHOT-jar-with-dependencies.jar cloudlab.ops.GoogleSheetsClient