[package]
name = "bencher"
version = "0.1.0"
authors = ["Gabriel Cardona <cgcardona@gmail.com>"]
edition = "2018"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]

[dev-dependencies]
criterion = "0.3"

[[bench]]
name = "my_benchmark"
harness = false
