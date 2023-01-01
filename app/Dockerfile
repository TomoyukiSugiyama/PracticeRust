# FROM rust:latest

# WORKDIR /usr/src/test-api
# COPY app .

# RUN cargo install --path .

# CMD ["test-api"]


FROM rust:latest

WORKDIR /app
COPY app/Cargo.toml Cargo.toml
RUN mkdir src/
RUN echo "fn main() {println!(\"if you see this, the build broke\")}" > src/main.rs
RUN cargo build --release
RUN rm -f target/release/deps/test-api*

COPY app/src src
RUN cargo install --path .

CMD ["test-api"]