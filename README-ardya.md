# Additional Note

Additional note from ardya

## Detailed steps to build winbox_dns_request

Tested on Ubuntu 22.04

```
sudo apt update
sudo apt upgrade -y
sudo apt install cmake
sudo apt install build-essential
sudo apt install libboost-all-dev
git clone https://github.com/suryadina/routeros
cd routeros/poc/winbox_dns_request/
mkdir build
cd build
cmake ..
make
```

After that, test the build
```
./winbox_dns_request -i 192.168.88.1 -p 8291 -s 8.8.8.8
```
