# Dockerfile for building byncoin binaries.

Now, you can build your own byncoin files on all systems with docker and do it easy without installing depends on your system.

## How:

### Build docker image

```
sudo docker build .
```

### Run docker container

Builder will return HASH of image
Example:
Successfully built 9bbff825d50f

```
sudo docker run -it -v ~/path/to/byncoin/folder:/byncoin 9bbff825d50f
```

If your system uses SELINUX you may use --privileged=true key

```
sudo docker run --privileged=true -it -v ~/development/byncoin:/byncoin 9bbff825d50f
```

See byncoin-qt file in used byncoin folder and byncoind file in src subfolder.