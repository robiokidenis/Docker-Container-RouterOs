# Docker ContainerRouterOs
This repository contains a Docker container for running x86_64 virtual machines using QEMU. It uses high-performance QEMU options (KVM, and TAP network driver).


## Running RouterOs CHR on docker container

## How to run
```bash
mkdir docker_routeros
cd docker_routeros
git clone https://github.com/robiokidenis/Docker-Container-RouterOs.git
docker-compose up --build
```

## To Check 
```bash
docker images
docker-compose ps


        Name                   Command           State                                                            Ports
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
docker-compose_chr_1   /routeros/entrypoint.sh   Up      0.0.0.0:1111->1194/tcp,:::1111->1194/tcp, 1701/tcp, 1723/tcp, 21/tcp, 0.0.0.0:2222->22/tcp,:::2222->22/tcp,
                                                         0.0.0.0:12223->23/tcp,:::12223->23/tcp, 443/tcp, 4500/udp, 50/tcp, 500/udp, 51/tcp, 5900/tcp,
                                                         0.0.0.0:12->80/tcp,:::1610->80/tcp, 0.0.0.0:1212->8291/tcp,:::1212->8291/tcp, 0.0.0.0:18728->8728/tcp,:::18728->8728/tcp,
                                                         0.0.0.0:18729->8729/tcp,:::18729->8729/tcp


```

## Exposed Ports

 ```bash {
                "1194/tcp": {},
                "1701/tcp": {},
                "1723/tcp": {},
                "21/tcp": {},
                "22/tcp": {},
                "23/tcp": {},
                "443/tcp": {},
                "4500/udp": {},
                "50/tcp": {},
                "500/udp": {},
                "51/tcp": {},
                "5900/tcp": {},
                "80/tcp": {},
                "8291/tcp": {},
                "8728/tcp": {},
                "8729/tcp": {}
           
```

 [link tutorial !](https://robiokidenis.medium.com/cara-running-mikrotik-routeros-di-docker-container-526007b2cea9) 

Thats's It :star_struck:
