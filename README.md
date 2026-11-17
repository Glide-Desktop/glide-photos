# Glide Photos

The photo library and viewer of the [Glide desktop](https://github.com/Glide-Desktop):
years / months / days, albums, favourites, a viewer with an info panel, and
basic editing.

## Build

```sh
cargo build --release
```

The shared crates come from a tag of
[glide-libs](https://github.com/Glide-Desktop/glide-libs). To build against a
checkout of glide-libs next to this one, create `.cargo/config.toml` (ignored
by git):

```toml
[patch."https://github.com/Glide-Desktop/glide-libs"]
glide-config = { path = "../glide-libs/crates/glide-config" }
glide-sdk = { path = "../glide-libs/crates/glide-sdk" }
```

Split from the Glide monorepo with its history in November 2026.
