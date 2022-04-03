# kali-nomachine
Kali Dockerfile with NoMachine remote access

# How to run
## Build

```
git clone https://github.com/GOBMi-ux/kali-nomachine.git
cd kali-nomachine
docker build -t=kali-nomachine .
```
## Docker pull command
```
docker pull GOBMi-ux/kali-nomachine
```

## Usage

```
docker run -d -p 4000:4000 --name desktop --cap-add=SYS_PTRACE moguay/kali-nomachine
```

## Connect to the container

Download the NoMachine client from: https://www.nomachine.com/download, install the client, create a new connection to your public ip, port 4000, NX protocol, use password for authentication (user: nomachine password: nomachine | change Dockerfile to use your own password)
