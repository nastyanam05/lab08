FROM ubuntu:latest
WORKDIR /app
COPY client.cpp /app/client.cpp
RUN apt-get update && \
    apt-get install  -y g++ && \
    g++ -o client client.cpp
EXPOSE 1223
CMD ["./client"]
