# basic python image
FROM python:3.7

# install pika to access rabbitmq
RUN pip install pika
RUN pip install requests
RUN pip install flask

# Without this setting, Python never prints anything out.
ENV PYTHONUNBUFFERED=1

# declare the source directory
WORKDIR /home/lawjarp/PESU/Projects/cc_hackathon/src/producer
# copy the file
COPY producer.py .

EXPOSE 5005
# start command
CMD [ "python", "producer.py"]