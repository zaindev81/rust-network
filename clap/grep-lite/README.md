# grep-lite

```sh
# Basic search
cargo run -- "error" log1.txt log2.txt

# With line numbers and case sensitivity
cargo run -- "Error" log1.txt --line-numbers --case-sensitive
cargo run -- "Error" log1.txt log2.txt --line-numbers --case-sensitive

# Count matches only
cargo run -- "warning" app.log --count

# Show non-matching lines
cargo run -- "debug" app.log --invert

# Combine flags
cargo run -- "exception" log1.txt log2.txt --line-numbers --case-sensitive --count
```