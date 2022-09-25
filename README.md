[Build new version](https://github.com/prashantv/tailscale-builds/actions/workflows/build.yaml)

Once the release is built, download using curl:
```console
$ VERSION=v1.30.2
$ rm tailscale tailscaled
$ curl -L -o tailscale https://github.com/prashantv/tailscale-builds/releases/download/$VERSION/tailscale-linux-armv5
$ curl -L -o tailscaled https://github.com/prashantv/tailscale-builds/releases/download/$VERSION/tailscaled-linux-armv5
$ chmod a+rx tailscale tailscaled

# restart tailscaled after replacing
```
