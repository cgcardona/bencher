# Bencher

Example app using Rust's benchmark framework [criterion](https://github.com/bheisler/criterion.rs) and [gnuplot](http://www.gnuplot.info).

## Installation

Clone the repo

```
git clone https://github.com/bheisler/criterion.rs.git
```

Change directories

```
cd criterion
```

Install dependencies and build app

```
cargo build
```

Run the benchmarks

```
cargo bench
    Finished release [optimized] target(s) in 0.09s
     Running target/release/deps/bencher-ef385ec0112399e3

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out

     Running target/release/deps/my_benchmark-44ff04d7dba46a3e
fib 20                  time:   [17.262 us 17.425 us 17.587 us]
                        change: [-4.2772% -1.0604% +2.3046%] (p = 0.55 > 0.05)
                        No change in performance detected.
Found 4 outliers among 100 measurements (4.00%)
  1 (1.00%) low mild
  3 (3.00%) high severe
```

View the plots

```
open target/criterion/report/index.html
```

![Chart 1](https://i.imgur.com/8PbDmDi.png "Chart 1")
![Chart 2](https://i.imgur.com/kSTHYJq.png "Chart 2")

## Benchmarks

All the actions is happening in [./benches/my_benchmark.rs]
