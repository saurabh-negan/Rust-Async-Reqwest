# 🌐 Rust Async Reqwest Example

A simple async Rust project that demonstrates how to perform HTTP GET requests using [reqwest](https://crates.io/crates/reqwest) and [tokio](https://tokio.rs/).  
It fetches data from an API endpoint and prints the status, headers, and body.

---

## 🚀 Features
- Asynchronous HTTP client with `reqwest`
- Uses `tokio` runtime for async execution
- Prints response status, headers, and body
- Configured with `rustls-tls` for secure HTTPS requests

---

## 📦 Dependencies, Run & Example Output

```bash
# Cargo.toml
[dependencies]
reqwest = { version = "0.11", features = ["json", "rustls-tls"] }
tokio = { version = "1", features = ["full"] }
anyhow = "1.0"
```
# Run the program
```
cargo run
```

# Example Output
```
Status: 200 OK
Headers:
{
    "content-type": "application/json",
    "content-length": "304",
    ...
}
Body:
{
  "args": {},
  "headers": {
    "accept": "*/*",
    "host": "httpbin.org",
    ...
  },
  "origin": "xx.xx.xx.xx",
  "url": "https://httpbin.org/get"
}
