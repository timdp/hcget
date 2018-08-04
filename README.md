# hcget

Downloads and installs the latest version of any
[Hashicorp](https://www.hashicorp.com/) product.

## Supported Platforms

Debian-compatible (including Ubuntu)

## Installation

Just download [`hcget`](hcget) and drop it somewhere under your `PATH`. Don't
forget to make it executable.

## Usage

```bash
$ hcget terraform
$ hcget packer
```

## Motivation

Hashicorp doesn't maintain a Debian repository for their tools. While you can
install them by "simply" downloading a zip file and extracting it, that quickly
becomes cumbersome.

Therefore, this little Bash script consults the official
[releases.hashicorp.com](https://releases.hashicorp.com/) endpoint to figure out
what the latest version of the desired tool is. If it's not already installed
under `/usr/local/bin`, it will subsequently download and extract the zip file.

## Author

[Tim De Pauw](https://tmdpw.eu/)

## License

MIT
