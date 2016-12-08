#Readme

You must choose a access key and secret key when launching Minio. They are set with the `MINIO_ACCESS_KEY` and `MINIO_SECRET_KEY` environment variables.

etcd needs to know the host ip. It is set with `HostIP` environment variable. Try

    HostIP=`curl ipinfo.io/ip`

To start the docker containers, use

    HostIP=`curl ipinfo.io/ip` \
    MINIO_ACCESS_KEY=AKIAIOSFODNN7EXAMPLE \
    MINIO_SECRET_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY \
    docker-compose up -d 
