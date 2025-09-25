``` shell
docker run -d --restart always --pull always \
  --name Mawari_node \
  -v ~/mawari:/app/cache \
  -e OWNERS_ALLOWLIST=$OWNER_ADDRESS \
  $MNTESTNET_IMAGE
```
