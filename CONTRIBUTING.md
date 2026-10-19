# Contributing

Bug reports, CT log quirks, and pull requests are welcome.

## Before you start

Open an [issue](https://github.com/reloading01/certstream-server-rust/issues) first for larger changes so the approach can be agreed before you write code. For a bug, include the version, your configuration, and the relevant log lines.

## Build and test

```bash
git clone https://github.com/reloading01/certstream-server-rust
cd certstream-server-rust
cargo build --release
cargo test --release
```

CI builds and tests with stable Rust.

## Pull requests

- Keep a pull request to one logical change.
- When you fix a bug, add a test that fails without the fix.
- If a change touches CT log fetching, parsing, or verification, also run it against live logs. Unit tests do not reproduce operator behaviour.
- Use [Conventional Commits](https://www.conventionalcommits.org/) for commit messages, for example `fix(ct): handle a missing checkpoint`.
- Describe why the change is needed and how you verified it.

## Other ways to help

Starring the repository or sharing it helps the project get found. You can also [sponsor it on GitHub](https://github.com/sponsors/reloading01).
