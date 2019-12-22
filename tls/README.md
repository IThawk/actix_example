# tls example

win10
set OPENSSL_LIB_DIR=C:/OpenSSL-Win64
set OPENSSL_INCLUDE_DIR=C:/OpenSSL-Win64/include
cargo build

包位置：.\examples\target\debug
## Usage

### server

```bash
cd examples/tls
cargo run (or ``cargo watch -x run``)
# Started http server: 127.0.0.1:8443
```

### web client

- curl: ``curl -v https://127.0.0.1:8443/index.html --compressed -k``
- browser: [https://127.0.0.1:8443/index.html](https://127.0.0.1:8443/index.html)
