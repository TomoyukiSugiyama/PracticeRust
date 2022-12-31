FROM rust:1.31

WORKDIR /usr/src/test-api
COPY app .

RUN cargo install --path .

CMD ["test-api"]