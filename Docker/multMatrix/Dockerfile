FROM ubuntu:20.04
RUN apt-get update
RUN apt-get install -y software-properties-common
RUN mkdir -p /home/ubuntu/multMatrix
EXPOSE 32000
COPY multMatrixServer /home/ubuntu/multMatrix/
RUN chmod +x /home/ubuntu/multMatrix/multMatrixServer
CMD /home/ubuntu/multMatrix/multMatrixServer
