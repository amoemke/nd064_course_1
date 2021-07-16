FROM golang:alpine
LABEL maintainer="Aurea Moemke"

#COPY . /go/src/app
WORKDIR /go/src/app
ADD . .

# command to run application
RUN go mod init
RUN go build -o helloworld

EXPOSE 6111

# command to run on container start
CMD [ "./helloworld" ]