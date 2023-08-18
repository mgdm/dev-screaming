# dev-screaming
Add a device called `/dev/screaming` on Linux. It provides infinite screaming, not unlike [@infinite_scream](https://botsin.space/@scream).

*Heavily* based on a [Stack Overflow answer by Mark Wagner](https://serverfault.com/a/1097608).

![A screenshot of the output](/screenshot.png?raw=true "Screenshot")

# How To

```bash
apt install build-essential linux-headers
git clone https://github.com/mgdm/dev-screaming.git
cd dev-screaming
make
insmod screaming.ko

dd if=/dev/screaming bs=512 count=1 status=none
```

