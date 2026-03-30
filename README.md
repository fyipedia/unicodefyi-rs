# unicodefyi

[![crates.io](https://img.shields.io/crates/v/unicodefyi.svg)](https://crates.io/crates/unicodefyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Unicode character lookup with 17 encodings — API client for [unicodefyi.com](https://unicodefyi.com).

> **Try the interactive tools at [unicodefyi.com](https://unicodefyi.com)**

## Install

`cargo add unicodefyi`

## Quick Start

```rust
use unicodefyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("snowflake").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install unicodefyi` | [PyPI](https://pypi.org/project/unicodefyi/) |
| **npm** | `npm install unicodefyi` | [npm](https://www.npmjs.com/package/unicodefyi) |
| **Go** | `go get github.com/fyipedia/unicodefyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/unicodefyi-go) |
| **Rust** | `cargo add unicodefyi` | [crates.io](https://crates.io/crates/unicodefyi) |
| **Ruby** | `gem install unicodefyi` | [rubygems](https://rubygems.org/gems/unicodefyi) |

## Embed Widget

Embed [UnicodeFYI](https://unicodefyi.com) widgets on any website with [unicodefyi-embed](https://widget.unicodefyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/unicodefyi-embed@1/dist/embed.min.js"></script>
<div data-unicodefyi="entity" data-slug="snowflake"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.unicodefyi.com)

## Links

- [UnicodeFYI](https://unicodefyi.com) — Main site
- [API Documentation](https://unicodefyi.com/developers/)
- [OpenAPI Spec](https://unicodefyi.com/api/openapi.json)
- [Glossary](https://unicodefyi.com/glossary/)

## License

MIT
