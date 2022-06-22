# SetupMachineForXDP
## Make your ubuntu 20 machine ready to use XDP programs.
Install the packages manually or `run init.sh`.

#### Setup libbpf
``` bash
git clone https://github.com/libbpf/libbpf
```
```bash
cd libbpf
```
```bash
git submodule update --init
```
----------------------------
#### Install packages
``` bash
sudo apt install clang llvm libelf-dev libpcap-dev gcc-multilib build-essential
```

``` bash
sudo apt install linux-tools-$(uname -r)
```

``` bash
sudo apt install linux-headers-$(uname -r)
```

``` bash
sudo apt install linux-tools-common linux-tools-generic
sudo apt install tcpdump
```

``` bash
git clone --depth 1 https://github.com/libbpf/libbpf
cd src
sudo make install
```

``` bash
sudo chmod 777 XDP_pack.sh
./XDP_pack.sh
```

``` bash
apt-get install -y pkg-config
```

### That's It
