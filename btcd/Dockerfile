FROM golang

RUN go get -u github.com/Masterminds/glide

RUN git clone https://github.com/btcsuite/btcd $GOPATH/src/github.com/btcsuite/btcd
RUN cd $GOPATH/src/github.com/btcsuite/btcd \
  && glide install \
  && go install ./cmd/..
ENTRYPOINT $GOPATH/bin/btcd

