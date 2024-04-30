# powx CLI
A command line interface for the powx program.

## Modify vs Ore CLI
- [`Cargo.toml`](cargo.toml) – Replaced ore-package with powx-program.
- [`mine.rs`](src/mine.rs) – Adjust bus reward return conditions.
- [`cu_limits.rs`](src/cu_limits.rs) – Adjust the limits of cu.

## Building
To build the powx CLI, you will need to have the Rust programming language installed. You can install Rust by following the instructions on the [Rust website](https://www.rust-lang.org/tools/install).

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
```
```
source ~/.bashrc
```

Once you have Rust installed, you can build the powx CLI by running the following command:

```sh
cargo build --release
```

## Example

Mine for powx
```
<YOUR_HOME>/powx-cli/target/release/powx --keypair <YOUR_KEY>.json --rpc <RPC> --priority-fee 100000 mine --threads 4
```

Claim for powx
```
<YOUR_HOME>/powx-cli/target/release/powx --keypair <YOUR_KEY>.json --rpc <RPC> --priority-fee 100000 claim
```

Reward for powx
```
<YOUR_HOME>/powx-cli/target/release/powx --keypair <YOUR_KEY>.json --rpc <RPC> rewards
```

Balance for powx
```
<YOUR_HOME>/powx-cli/target/release/powx --keypair <YOUR_KEY>.json --rpc <RPC> balance
```