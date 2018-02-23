FROM ubuntu

RUN apt update -y && apt upgrade -y && \
    apt install -y \
        tmux ssh git vlock wget curl zsh vim linux-tools-generic tree atop htop glances sysdig sysstat
RUN curl -sL https://deb.nodesource.com/setup_9.x | bash - && apt-get install -y nodejs
RUN npm install -g autocannon  

CMD tail -f /dev/null
