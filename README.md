# Immich server configuration

Key points:

- No reverse proxy. I will be using tailscale services to access the server remotely, so no need for nginx or caddy.
- Upload data will be an NFS share mounted at /mnt/immich
- DB will be stored in docker volume.
- DB dumps will be stored in S3 Bucket, and handled by greenmask container.
