FROM ubuntu:latest
WORKDIR /app
COPY server.cpp /app/server.cpp
RUN apt-get update && \
    apt-get install  -y g++ && \
    g++ -o server server.cpp
EXPOSE 1223
CMD ["./server"]
