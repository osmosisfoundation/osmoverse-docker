FROM rocker/verse:latest
MAINTAINER "Devin Pastoor" devin.pastoor@gmail.com

## littler installGithub should be simlinked already 
# from the base R image
RUN installGithub.r --deps TRUE \
    dpastoor/phmxversecore
    