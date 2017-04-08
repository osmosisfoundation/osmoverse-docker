FROM osmoverse/phmxcore:latest
MAINTAINER "Devin Pastoor" devin.pastoor@gmail.com

## littler installGithub should be simlinked already 
# from the base R image
RUN git clone https://github.com/stan-dev/cmdstan.git \
     && cd cmdstan \
     && git checkout release/v2.14.0 \
     &&  git clone https://github.com/charlesm93/stan.git \
     &&  rm -r stan_2.14.0 \
     &&  mv stan stan_2.14.0 \
     &&  cd stan_2.14.0 \
     &&  git checkout torsten-develop \
     &&  mkdir lib \
     &&  cd lib \
     &&  git clone https://github.com/charlesm93/math.git \
     &&  mv math stan_math_2.14.0 \
     &&  cd stan_math_2.14.0 \
     &&  git checkout torsten-develop 
     
 RUN cd /cmdstan \
   && make build
