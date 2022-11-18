# substrate-api-client

<p align="center">
<img src=./web3_foundation_grants_badge_black.svg width = 400>
</p>

substrate-api-client a library written in Rust for connecting to the substrate's RPC interface via WebSockets allowing to

* Compose extrinsics, send them and subscribe to updates (synchronously).


To execute the examples, a running substrate node is needed. You can download a node artifact from substrate directly: https://github.com/paritytech
```


To run an example, clone the `substrate-api-client` repository and run the desired example directly with the cargo command:

```
or download the already built binaries from Github Actions: https://github.com/scs/substrate-api-client/actions and run them without any building:

```bash
chmod +x <example>
./<example>
```
 by prepending `RUST_LOG=info` or `RUST_LOG=debug`.

The following examples can be found in the [examples](/examples) folder:

* [example_benchmark_bulk_xt](/examples/example_benchmark_bulk_xt.rs): Float the node with a series of transactions.
* [example_compose_extrinsic_offline](/examples/example_compose_extrinsic_offline.rs): Compose an extrinsic without interacting with the node.
* [example_contract_instantiate_with_code](/examples/example_contract_instantiate_with_code.rs): Instantiate a contract on the chain.
* [example_contract](/examples/example_contract.rs): Handle ink! contracts (put, create, and call). **DEPRECATED!**
* [example_custom_storage_struct](/examples/example_custom_storage_struct.rs): Fetch and decode custom structs from the runtime. **DEPRECATED!**
* [example_event_callback](/examples/example_event_callback.rs): Subscribe and react on events.
* [example_event_error_details](/examples/example_event_error_details.rs): Listen to error events from the node to determine if an extrinsic was successful or not.
* [example_generic_event_callback](/examples/example_generic_event_callback.rs): Listen to an example event from the node.
* [example_generic_extrinsic](/examples/example_generic_extrinsic.rs): Compose an extrinsic for any call in any module by supplying the module and call name as strings.
* [example_get_block](/examples/example_get_block.rs): Read header, block and signed block from storage.
* [example_get_storage](/examples/example_get_storage.rs): Read storage values.
* [example_print_metadata](/examples/example_print_metadata.rs): Print the metadata of the node in a readable way.
* [example_sudo](/examples/example_sudo.rs): Create and send a sudo wrapped call.
* [example_transfer_using_seed](/examples/example_transfer_using_seed.rs): Transfer tokens by using a wrapper of compose_extrinsic with an account generated with a seed.

## Alternatives

Parity offers a Rust client with similar functionality: https://github.com/paritytech/substrate-subxt

## Acknowledgements

The development of substrate-api-client is financed by [web3 foundation](https://web3.foundation/)'s grant programme.

We also thank the teams at

* [Parity Technologies](https://www.parity.io/) for building [substrate](https://github.com/paritytech/substrate) and supporting us during development.
