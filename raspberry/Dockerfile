FROM raspbian:latest
MAINTAINER https://github.com/ivanpl82
LABEL version="1.0"
LABEL description="Setting environment"

#upgrade system and install python 3
RUN sudo apt-get update
RUN sudo apt-get remove --purge -y python
RUN sudo apt-get autoremove -y
RUN sudo apt-get upgrade -y
RUN sudo apt-get install -y file python3 pip 

#setting alias
echo "export LS_OPTIONS='--color=auto'">>~/.bashrc
echo "alias ll='ls $LS_OPTIONS -l'">>~/.bashrc
echo "alias python='python3'">>~/.bashrc
