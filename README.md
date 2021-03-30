# Installation
## Install Docker & Git

```bash
apt update
apt install -y docker docker-ce docker.io git
```

## Clone the Repositorie

```bash
git clone https://github.com/cva6thales/cva6thales
```

## Install Docker Container

```bash
cd cva6thales/
./install
```

> Attention: The installation may take more than 1 hour. Step 2 (toolchain-builder) is the longest, about 40 minutes.

## Run and exec Docker Container

```bash
# RUN
docker run -dti \
  --name verilator-spike \
  --hostname verilator-spike \
  riscv-debian-buster:ci-platform-verilator-spike

# EXEC
docker exec -ti verilator-spike bash
```
