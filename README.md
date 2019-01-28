# Wallet713 in a Docker Container

## Installation 1 - Build Yourself (RECOMMENDED)

This is the recommended way. You can see what it is in in the Dockerfile, and
don't need to trust in me, just wallet713 developers (https://github.com/vault713/wallet713).

Make sure you have docker installed, then, clone this repo. In this repo
directory, type:

```bash
docker build -t wallet713 .
```
Once built, 

### To run from Linux:
```bash
docker run -it -v $(pwd):/root/.wallet713 --rm wallet713
```

### To run from Windows:
```bash
docker run -it -v %cd%:/root/.wallet713 --rm wallet713
```

The wallet will use the current directory to store the mainnet/floonet data (main/floo directories).

## Installation 2 - Run from Hub
This one is fairly straightforward. You're running the image from the automated
builds of this repo.

### From Linux:

```bash
docker run -it -v $(pwd):/root/.wallet713 --rm mpenagar/wallet713
```

### From Windows:

```bash
docker run -it -v %cd%:/root/.wallet713 --rm mpenagar/wallet713
```

The wallet will use the current directory to store the mainnet/floonet data (main/floo directories).
