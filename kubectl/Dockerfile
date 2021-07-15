FROM alpine:latest

RUN apk add python3 py3-pip curl

RUN curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

RUN chmod u+x kubectl && mv kubectl /bin/kubectl

CMD kubectl version --client
