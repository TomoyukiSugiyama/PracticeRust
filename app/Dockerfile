FROM rust:1.31

WORKDIR /usr/src/test-api
COPY . .

RUN cargo install --path .

CMD ["test-api"]