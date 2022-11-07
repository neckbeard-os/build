# Build
A repository for testing builds and buildscripts with GitHub workflow & actions as well as Docker images and whatnot else we can think of that we want to try out

It might evolve into something else in time, we'll see

☆ RISC-V

☆ Docker

☆ GCC

☆ Musl libc

TODO:

☆ Toybox

☆ Compiler (perhaps?)

## GitHub Codespace

If you have started a new GitHub Codespace Debian container, which is configured in the `devcontainer.json`, run the command below to be able to build the GNU RISC-V Toolchain. It's might be a good idea to run it at first boot either way so there won't be any issues when building, annoying to have the build fail due to missing packages. 

```bash
sudo apt-get update -y && \
sudo apt-get install -y autoconf automake autotools-dev curl python3 \
libmpc-dev libmpfr-dev libgmp-dev libtool zlib1g-dev libexpat-dev \
gawk build-essential bison flex texinfo gperf patchutils bc
```
