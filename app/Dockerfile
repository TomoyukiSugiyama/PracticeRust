FROM rust:1.31

WORKDIR /usr/src/test-api
COPY ./src .

RUN cargo install --path .

CMD ["test-api"]