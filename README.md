# Sei Binaries

This repository provides pre-built `seid` binaries extracted from the [sei-chain repository](https://github.com/sei-protocol/sei-chain). These binaries are fully self-contained—with the [libwasmvm](https://github.com/CosmWasm/wasmvm) library statically linked—so you don't need to install any additional libraries to run them.

## Features

- **Pre-built Binaries:** Use `seid` without building from source.
- **Statically Linked Dependencies:** The binaries include a statically linked libwasmvm, ensuring a hassle-free experience.
- **Optimized for Sei-Chain:** Designed specifically for the Sei blockchain ecosystem.

## Installation

### Option 1: Direct Binary Installation

1. **Download the Binary:**
   Visit the [Releases](https://github.com/alexander-sei/sei-binaries/releases) page to download the appropriate binary for your operating system.

2. **Set Executable Permissions (Linux/macOS):**
   ```bash
   chmod +x seid
   ```

3. **Move to System Path (Optional):**
   ```bash
   sudo mv seid /usr/local/bin/
   ```

4. **Verify Installation:**
   ```bash
   seid version
   ```

### Option 2: Installing via APT (Debian/Ubuntu)

1. **Download the .deb Package:**
   Visit the [Releases](https://github.com/alexander-sei/sei-binaries/releases) page and download the latest .deb package.

2. **Install using APT:**
   ```bash copy
   sudo apt install ./sei-chain_xyz.deb
   ```
   Replace `xyz` with the actual version you want to install.

   Alternatively, you can use `dpkg`:
   ```bash copy
   sudo dpkg -i ./sei-chain_xyz.deb
   ```

3. **Verify Installation:**
   ```bash copy
   seid version
   ```

## Usage

After installation, you can interact with the Sei blockchain using the `seid` binary. For a list of available commands and options, run:

```bash copy
seid --help
```

## Building from Source

If you prefer to build `seid` from the source code, please refer to the [sei-chain repository](https://github.com/sei-protocol/sei-chain) for comprehensive build instructions. Remember that the provided binaries are statically linked with libwasmvm, so no extra dependencies are required post-build.

## Troubleshooting

If you encounter any issues during installation or usage:

1. Ensure the binary has the correct permissions.
2. Verify you're using the correct binary for your operating system and architecture.
3. Check for any error messages when running commands.

## Contributing

Contributions to improve these binaries or update build processes are welcome. Please open an issue or submit a pull request if you have any enhancements or find any problems.

## License

This project is licensed under the terms specified in the [sei-chain repository](https://github.com/sei-protocol/sei-chain).
