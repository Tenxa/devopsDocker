FROM ubuntu:20.04

# Install curl
RUN apt-get update \
  && apt-get install -y curl

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh.
COPY input.sh .

# Grant permission to file
RUN chmod +x input.sh

# When running Docker run the command will be ./hello.sh
CMD ./input.sh
