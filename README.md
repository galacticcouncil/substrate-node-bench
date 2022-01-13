# Substrate node bench

node-bench utility to perform various benchmarks of a Substrate node.

Forked from Substrate repository. 

node-runtime updated to benchmark extrinsic overhead with Basilisk's changes.

Custom runtime includes:

- Basilisk's multi payment pallet 
- Basilisk's xyk pallet
- orml tokens, orml currencies

To benchmark extrinsic overhead, run:

```
cargo run --release -p node-bench -- ::node::import::wasm::sr25519::noop::rocksdb::custom --transactions 10000
```