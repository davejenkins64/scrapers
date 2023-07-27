# Start here: https://hub.docker.com/_/perl

# Using a perl image, be able to do development on files in this directory
# and subdirectories

# "Do development" can mean editing outside of container and running inside
# or executing the container and editing inside.

# First approach is to edit outside the container, just run inside

# At the time 5.38.0 was latest
FROM perl:latest
COPY . /usr/src/perl-scraper
WORKDIR /usr/src/perl-scraper
CMD [ "perl", "-v" ]

# Then to build and run:
#$ docker build -t perl-scraper .
#$ docker run -it --rm --name my-running-perl-scraper perl-scraper
