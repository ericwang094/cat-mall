## How to install linux on Windows

The official documentation is pretty clear on how to install wsl on Windows.

What I am interested is that how can I install multiple linux on the same machine since it is a good learning practice for 
future microservices project.

Mainly followed by this [doc](https://cloudbytes.dev/snippets/how-to-install-multiple-instances-of-ubuntu-in-wsl2)

Basically

1. download the linux distribution version you want to use. In my case, it is ubuntu.
download the image from this [link](https://cloud-images.ubuntu.com/releases/releases/22.04/release/ubuntu-22.04-server-cloudimg-amd64-wsl.rootfs.tar.gz)
Be aware, the link provided in the doc is different as above. the image in the doc is end of life stage.
2. then create three folders locally to serve as home dir.
1. run following command in powershell
```
wsl --import ubuntu-main "D:\IT\wsl-storage\ubuntu-main" C:\Users\ericw\Desktop\ubuntu-22.04-server-cloudimg-amd64-wsl.rootfs.tar.gz
wsl --import ubuntu-1 "D:\IT\wsl-storage\ubuntu-1" C:\Users\ericw\Desktop\ubuntu-22.04-server-cloudimg-amd64-wsl.rootfs.tar.gz
wsl --import ubuntu-2 "D:\IT\wsl-storage\ubuntu-2" C:\Users\ericw\Desktop\ubuntu-22.04-server-cloudimg-amd64-wsl.rootfs.tar.gz
``` 

## Enable docker on WSL

The easiest way is actually using docker-desktop, it is naturally integrated WSL with docker. [doc](https://docs.docker.com/desktop/windows/wsl/)