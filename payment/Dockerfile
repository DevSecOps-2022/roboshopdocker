FROM python:3
RUN mkdir -p /app
WORKDIR /app
COPY requirements.txt .
COPY payment.ini .
COPY *.py .
RUN pip install -r requirements.txt
ENV CART_HOST=cart
ENV CART_PORT=8080
ENV USER_HOST=user
ENV USER_PORT=8080
ENV AMQP_HOST=rabbitmq
ENV AMQP_USER=roboshop
ENV AMQP_PASS=roboshop123
