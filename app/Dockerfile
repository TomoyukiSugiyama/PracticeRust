FROM rust:latest

WORKDIR /usr/src/test-api
COPY app .

RUN cargo install --path .

CMD ["test-api"]

## ref: https://github.com/rust-lang/cargo/issues/2644
# FROM rust:latest

# WORKDIR /usr/src/app
# COPY app/Cargo.toml Cargo.toml
# RUN mkdir src/
# RUN echo "fn main() {println!(\"if you see this, the build broke\")}" > src/main.rs
# RUN cargo build --release --deps
# RUN rm -f target/release/deps/test-api*

# COPY app/src src
# RUN cargo build --release

# CMD ["/usr/local/cargo/bin/test-api"]
