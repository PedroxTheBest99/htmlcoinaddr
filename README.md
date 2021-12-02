# HTMLCOIN Address Converter

The address in bytes is `ripemd160(sha256(pubkey))`. This address could be encoded either with hex or base58.

# Demo

Install

```
go get -u github.com/htmlcoin/htmlcoinaddr
```

Convert hex address to base58 address (test net):

```
htmlcoinaddr --hex fe59cbc1704e89a698571413a81f0de9d8f00c69 --test
hgkGMtMJbK921UZpwYt3bMhE9d7nNMyUcC
```

Convert hex address to base58 address (main net):

```
htmlcoinaddr --hex fe59cbc1704e89a698571413a81f0de9d8f00c69
HjnsK9sSa8QhJbvTRYEHXapT8M9JHhSLqY
```

Convert base58 address to hex address:

```
htmlcoinaddr --base58 hgkGMtMJbK921UZpwYt3bMhE9d7nNMyUcC
fe59cbc1704e89a698571413a81f0de9d8f00c69
```

```
htmlcoinaddr --base58 HjnsK9sSa8QhJbvTRYEHXapT8M9JHhSLqY
fe59cbc1704e89a698571413a81f0de9d8f00c69
```

## Help

```
usage: htmlcoinaddr [<flags>]

Flags:
      --help           Show context-sensitive help (also try --help-long and --help-man).
  -h, --hex=HEX        address to convert in hex
  -b, --base58=BASE58  address to convert in hex
  -t, --test           generate base58 address for testnet
```
