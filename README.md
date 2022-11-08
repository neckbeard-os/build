# Build
A repository for testing builds and buildscripts with GitHub workflow & actions as well as Docker images and whatnot else we can think of that we want to try out. It might evolve into something else in time, we'll see

---

☆ RISC-V

☆ Docker

☆ GCC Cross-compiler

☆ Musl libc cross-compiler × _Thanks to [musl-cross-make][musl-cross-make] by [Rich Felker][richfelker]_

☆ RISC-V GNU Toolchain × _Thanks to [RISCV-GNU-Toolchain][riscv-gnu-toolchain] by [RISC-V Software Collaboration][riscv-collab]_

[musl-cross-make]: https://github.com/richfelker/musl-cross-make

[richfelker]: https://github.com/richfelker

[riscv-gnu-toolchain]: https://github.com/riscv-collab/riscv-gnu-toolchain

[riscv-collab]: https://github.com/riscv-collab

TODO:

☆ Toybox × _Thanks to [Rob Landley][landley], creator and maintainer of [Toybox][toybox]_

_Note: If you haven't heard of the Toybox project before or Rob Landley, I highly recommend looking them up_

<!-- LINKS -->

[toybox]: https://github.com/landley/toybox

[landley]: https://github.com/landley

<!-- LINKS END -->

A couple interesting & recommended YouTube videos to check out with Rob Landley for anyone interested. 

[Tutorial: Building the Simplest Possible Linux System - Rob Landley][seminarium-2017] _The Linux Foundation, 2017_

[Interview with Rob Landley, creator of toybox][interview-2017] _Toca do Tux, 2017_

[Toybox vs BusyBox - Rob Landley, hobbyist][seminarium-2019] _The Linux Foundation, 2019_

<!-- LINKS -->

[seminarium-2017]: https://www.youtube.com/watch?v=Sk9TatW9ino

[interview-2017]: https://www.youtube.com/watch?v=j7kk-_uuRFc

[seminarium-2019]: https://www.youtube.com/watch?v=MkJkyMuBm3g

<!-- LINKS END -->

☆ Compiler (perhaps?)

## GitHub Codespace Devcontainer

If you have started a new GitHub Codespace Debian container, which is configured in the `.devcontainer/devcontainer.json`, run the command below to be able to build the GNU RISC-V Toolchain. 

It might be a good idea to run it at first boot either way so there won't be any issues when building, annoying to have the build fail due to missing packages. 

```bash
sudo apt-get update -y && \
sudo apt-get install -y autoconf automake autotools-dev curl python3 \
libmpc-dev libmpfr-dev libgmp-dev libtool zlib1g-dev libexpat-dev \
gawk build-essential bison flex texinfo gperf patchutils bc
```
