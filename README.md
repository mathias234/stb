# stb

[![Crate](https://img.shields.io/crates/v/stb.svg)](https://crates.io/crates/stb)
![CI](https://github.com/mxpv/stb/workflows/CI/badge.svg)
[![Docs](https://docs.rs/stb/badge.svg)](https://docs.rs/stb)
![Crates.io](https://img.shields.io/crates/l/stb)


All in one safe Rust API and wrappers for [stb libraries](https://github.com/nothings/stb).

The following APIs are currently available:
- `stb_easy_font`
- `stb_dxt`
- `stb_image`
- `stb_image_write`
- `stb_perlin`

Please refer to the [documentation](https://docs.rs/stb) for details or have a look on [examples](https://github.com/mxpv/stb/tree/master/stb/examples).

In progress:
- `stb_truetype`

Not implemented, but planned:
- `stb_image_resize`
- `stb_rect_pack`

## Usage

Add the following to your `Cargo.toml` file:

```toml
[dependencies]
stb = "0.3.2"
```

or if you want to have a specific feature selection:

```toml
[dependencies]
stb = { version = "0.3.2", default-features = false, features = ["stb_easy_font"] }
```

## Create features
Here is the list of feature toggles available in this crate so far:
- `stb_easy_font`
- `stb_dxt`
    * `stb_dxt_use_rounding_bias`
- `stb_image`
    * `stbi_no_linear`
    * `stbi_no_jpeg`
    * `stbi_no_png`
    * `stbi_no_bmp`
    * `stbi_no_psd`
    * `stbi_no_gif`
    * `stbi_no_hdr`
    * `stbi_no_pic`
    * `stbi_no_pnm`
- `stb_image_write`
- `stb_perlin`

## Contributing

Contributions are generally welcome. Make sure your changes make sense for this project (if in doubt, open an issue first),
the code is reasonbly tested, and passes the CI checks.
