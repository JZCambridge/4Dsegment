# pre-built image
FROM jinmingduan/segmentationcoregistration:latest

# Set the working directory in the container
WORKDIR /root/segmentfd

RUN apt-get update && apt-get install -y build-essential git libjpeg-dev && \
    apt-get install -y vim tmux curl

COPY . .

# Make port 6666 available to the world outside this container (if needed)
EXPOSE 6666

# Set the entrypoint
ENTRYPOINT ["python3"]


