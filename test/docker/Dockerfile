FROM golang:1.13-stretch

# Copy SDK code into the container
RUN mkdir -p $HOME/go-algorand-sdk
COPY . $HOME/go-algorand-sdk
WORKDIR $HOME/go-algorand-sdk

# Run integration tests
CMD ["/bin/bash", "-c", "make unit && make integration"]
