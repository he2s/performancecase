FROM ubuntu

RUN apt update -y && apt upgrade -y && \
    apt install -y \
        tmux ssh git vlock wget curl zsh vim linux-tools-generic tree atop htop glances sysdig sysstat
RUN curl -sL https://deb.nodesource.com/setup_9.x | bash - && apt-get install -y nodejs
RUN apt install -y linux-tools-4.13.0-32-generic
RUN npm install -g autocannon  
RUN apt install -y strace ltrace
RUN apt autoremove; apt clean

CMD tail -f /dev/null
