FROM maven:3.9.16
RUN mkdir -p /app
WORKDIR /app
COPY pom.xml .
COPY src ./src
RUN mvn clean package
RUN mv target/shipping-1.0.jar shipping.jar
ENV CART_ENDPOINT=cart:8080
ENV DB_HOST=mysql
CMD ["java", "shipping.jar"]
# CMD ["sleep", "1000"]   