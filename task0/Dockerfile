# gets latest version of Ubuntu
FROM ubuntu:latest

# Set non-interactive frontend at the beginning
ENV DEBIAN_FRONTEND=noninteractive

# updates APT package index
RUN apt-get update

# upgrades currently installed software
RUN apt-get upgrade -y

# clean up, best practice - rm (remove files) 
# -rf ("recursive" deletes directories and all their contents/"force" doesn't ask for confirmation, ignores warnings, won't stop if some files don't exist)
# Removes the package lists since we're done with them
RUN apt-get clean && rm -rf /var/lib/apt/lists/*

# sets the default command to echo "Hello, World!"
CMD ["Hello, World!"]
