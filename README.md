# Parallel

SOCKS5 parallel racing aggregator

## Usage

### Config file mode

```json
{
  "listeners": [
    {
      "listen": "127.0.0.1:1080",
      "socks": ["upstream1:1081", "upstream2:1082"]
    }
  ]
}
```

```bash
go run .
```

### Command line mode

```bash
go run . --listen-address 127.0.0.1 --listen-port 1080 --socks upstream1:1081 --socks upstream2:1082
```

## Build

```bash
go build -o parallel
```
