# install-gns3-linux-mint

---

Core :

```
sudo add-apt-repository ppa:gns3/ppa
sudo apt update
sudo apt install gns3-gui gns3-server
```

IOU support :

```
sudo dpkg --add-architecture i386
sudo apt update
sudo apt install gns3-iou
```

Remove OLD docker Version :

```
sudo apt remove docker docker-engine docker.io
sudo snap remove docker
```

Tahap selanjutnya install docker, anda bisa lihat disini https://github.com/ndeso17/docker-linux-mint

Setelah berhasil menginstall docker, inilah perintah terakhir nya :

```
sudo usermod -aG ubridge,libvirt,kvm,wireshark,docker $(whoami)
```

Tutorial untuk Distro Linux lainnya ada disini : https://docs.gns3.com/docs/getting-started/installation/linux/
