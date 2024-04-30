FROM ubuntu
MAINTAINER Prashansa Kulshrestha
RUN apt-get update
RUN apt-get install -y python3
ADD hello-world.py /home/hello-world.py
CMD ["/home/hello-world.py"]
ENTRYPOINT ["python3"]