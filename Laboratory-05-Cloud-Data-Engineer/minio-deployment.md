# MinIO Deployment Documentation

## Docker Command Used

I used Docker to deploy the MinIO Object Storage server in the KillerCoda Ubuntu environment. This is the command that successfully worked:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"
```

The command created a container named `minio-server`. The MinIO image was downloaded from `quay.io` because the original image source was not available in my environment.

## Port Used for Web Console

I used **port 9001** to open the MinIO Web Console through the KillerCoda Traffic/Ports feature.

Port **9000** is used for the MinIO API, while port **9001** is used for the Web Console.

## Bucket Name

The bucket I created was:

**`client-photos`**

I used this bucket to store and test a sample file. The uploaded file confirmed that the MinIO storage server was working properly.

## Environment Variables

The `-e` flags are used to set environment variables for MinIO.

* `MINIO_ROOT_USER=cloudadmin` sets the username for the MinIO administrator account.
* `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the password for the administrator account.

These settings were used when starting the MinIO server so I could log in to the Web Console.

## Deployment Verification

To check if MinIO was running, I used:

```bash
docker ps
```

The command showed that the `minio-server` container was **Up** and that ports **9000** and **9001** were successfully mapped.

