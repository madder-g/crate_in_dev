# Setup

Before running `cargo`: 

setup your config file at the root of the project to set the default registry to our private registry.

```sh
./.cargo/config
```

```toml
[source.crates-io]
replace-with = "private_registry"

[source.private_registry]
registry = "sparse+https://raw.githubusercontent.com/madder-g/private_crates/main/"
```

Then you can run `cargo run`
