## DigiByte public testnet node

- Node
  - RPC Port 16101, Username: user, Password: pass

### To run this image with internal ports exposed at host:

```bash
docker run -it -d -p 16101:16101 coinfoundry/digibyte-public-testnet
```

### Example RPC against Node-Pool:

```bash
curl --user user:pass --data-binary '{"jsonrpc": "1.0", "id":"curltest", "method": "getinfo", "params": [] }' -H 'content-type: application/json;' http://127.0.0.1:16101/
```
