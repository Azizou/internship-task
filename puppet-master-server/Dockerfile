# This is a Dockerfile to create an image with the puppet master installed
# It expose network access to puppet
# Also note that it is based on the ubuntu 12.04 image

# VERSION		1.0

# Use the ubuntu 12.04 image provided by dotCloud

FROM ubuntu:12.04

# Maintainer

MAINTAINER Azizou Ogbone ogbazi001@myuct.ac.za

#Ensure the package repository is up to date

RUN echo "wget https://apt.puppetlabs.com/puppetlabs-release-precise.deb" > /etc/apt/source.list

# run the update

RUN apt-get update

#install nano and ssh as tools to edit and debug remotely remote

RUN apt-get install nano

#Install puppetmaster

RUN apt-get install -y puppetmaster

#Expose puppetmaster port 8140 to network

EXPOSE 8140
