``` shell
docker run -d --restart always --pull always \
  --name Mawari_node \
  -v ~/mawari:/app/cache \
  -e OWNERS_ALLOWLIST=$OWNER_ADDRESS \
  $MNTESTNET_IMAGE
```

``` shell
~/mawari# docker exec -it Mawari_node sh
/app # ls -l
total 24420
drwxr-xr-x    2 root     root          4096 Sep 25 14:27 cache
-rw-r--r--    1 root     root           381 Sep 15 13:32 config.yml
-rwxr-xr-x    1 root     root      24991840 Sep 15 13:34 node
drwxr-xr-x    2 root     root          4096 Sep 15 13:34 plugins
```

``` shell
/app # cat cache/flohive-cache.json
{
  "burnerWallet": {
    "privateKey": "",
    "address": ""
  }
```
