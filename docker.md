Change the docker data location to another disk
```
wsl --export docker-desktop-data "E:\docker\docker-desktop-data.tar"
wsl --unregister docker-desktop-data
wsl --import docker-desktop-data "E:\docker" "E:\docker\docker-desktop-data.tar" --version 2
```
