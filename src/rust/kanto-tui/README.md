# Kanto Container Management TUI

A simple ncurses-TUI for kanto-cm that allows for easier management of deployed containers. Supports mouse and keyboard interaction.

# Usage

 To get started:

```bash
kantui --help
```

![Screenshot](misc/kantocmcurses-ss.png)

NCurses controls the stdout and cleans up on exit/crash. Thus to capture (if needed) error messages:

```bash
RUST_BACKTRACE=1 kantui 2> stderr.log
```

# Building

```bash
cd src/rust/kanto-tui
git submodule init
git submodule update
cargo build --release
```