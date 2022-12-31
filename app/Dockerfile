FROM rust:latest

WORKDIR /usr/src/test-api
COPY app .

RUN cargo install --path .

CMD ["test-api"]