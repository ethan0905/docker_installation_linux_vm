# docker_installation_linux_vm

1. Remove existing version
```bash
sudo apt-get remove docker docker-engine docker.io containerd runc
```
2. update packages
```bash
sudo apt-get update
```
3. install necessary dependencies
```bash
sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release
```
4. install docker and run the installation script using curl
```bash
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```
5. add your user to the docker group and run docker command without using sudo
```bash
sudo usermod -aG docker $USER
```
6. Log out of your session and log back in for the group changes to take effect.
