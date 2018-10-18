FROM jenkins/jenkins:lts

USER root


RUN curl https://download.docker.com/linux/static/stable/x86_64/docker-18.06.1-ce.tgz \
    | tar xvz docker/docker \
    && mv docker/docker /usr/local/bin/docker \
    && rm -rf docker \
    && curl -L \
        "https://github.com/docker/compose/releases/download/1.22.0/docker-compose-$(uname -s)-$(uname -m)" \
        -o /usr/local/bin/docker-compose \
    && chmod +x /usr/local/bin/docker-compose
