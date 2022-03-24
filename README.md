# near-protocol demo smartcontract

## Build
```commandline
$ cargo build --target wasm32-unknown-unknown --release
```

## Deploy
```commandline
$ near login
$ near deploy --wasmFile target/wasm32-unknown-unknown/release/near_demo.wasm --accountId account.testnet
```

## Usage
Get number
```commandline
$ near view account.testnet get_num --accountId account.testnet
```

Increament number
```commandline
$ near call account.testnet increment --accountId account.testnet
```