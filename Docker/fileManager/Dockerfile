FROM ubuntu:20.04
RUN apt-get update
RUN apt-get install -y software-properties-common
RUN mkdir -p /home/ubuntu/fileManager
RUN mkdir -p /home/ubuntu/dirprueba
RUN echo "hola dir a!" > /home/ubuntu/dirprueba/a.txt
RUN echo "hola dir b!" > /home/ubuntu/dirprueba/b.txt
RUN echo "hola dir c!" > /home/ubuntu/dirprueba/c.txt
EXPOSE 30003
COPY fileManager/fileManagerServer /home/ubuntu/fileManager/ 
RUN chmod +x /home/ubuntu/fileManager/fileManagerServer /home/ubuntu/dirprueba/a.txt /home/ubuntu/dirprueba/b.txt /home/ubuntu/dirprueba/c.txt
CMD /home/ubuntu/fileManager/fileManagerServer 
