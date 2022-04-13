# simple-proxy

This is a simple proxy written in [Go](https://golang.org).

## Prerequisites

* Go 1.3.3, or a compatible version

## Usage
Choose one of of the methods bellow, either way the proxy will be running on port `8080`

### Using regular Go

```bash
go run simple-proxy.go
```
### Using EGo in simulation mode

```bash
# If your hardware does not support SGX, enable simulation mode with this command:
export OE_SIMULATION=1

ego-go build simple-proxy.go
ego sign simple-proxy
ego run simple-proxy
```
