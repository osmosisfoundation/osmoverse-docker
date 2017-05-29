FROM rocker/verse:latest
MAINTAINER "Devin Pastoor" devin.pastoor@gmail.com

## littler installGithub should be simlinked already 
# from the base R image
RUN wget https://gist.githubusercontent.com/dpastoor/0bf40c3d0df2ef5bd961dd3acf5aa0bf/raw/28dde0f7e186159ac924f87dd644eda8766d0437/install_github.r -O install_github.r \
  && chmod +x install_github.r

RUN ./install_github.r dpastoor/phmxversecore 
    
