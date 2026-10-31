# SigmaOS boot_config

A Rust model for boot-menu settings, kernel parameters, and boot entries. It formats command-line parameters and generates GRUB-style configuration text in memory.

It does not install a bootloader, write system boot files, or verify that generated configuration works on a machine. `SigmaOS-boot_config` is a separate repository from `SigmaOS-boot-config` despite the similar names.

## Build

The manifest references sibling [`SigmaOS-kernel`](../SigmaOS-kernel). From the SigmaOS checkout:

```sh
cargo check --manifest-path SigmaOS-boot_config/Cargo.toml --lib
```

## License

GPL-3.0-or-later. See [`Cargo.toml`](Cargo.toml).
