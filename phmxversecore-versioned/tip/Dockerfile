FROM osmoverse/phmxcore:latest
MAINTAINER "Devin Pastoor" devin.pastoor@gmail.com

## littler installGithub should be simlinked already 
# from the base R image
RUN install2.r bindrcpp \
&& ./install_github.r \
    tidyverse/dplyr tidyverse/tidyr tidyverse/purrr hadley/purrrlyr
    