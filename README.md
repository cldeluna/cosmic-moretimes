## NetDevOps
#### 2019-11-22 claudia@indigowire.net

## Cosmic Cuttlefish Ansible 2.8 "How Many More Times" Dockerfile
 - Latest Ubuntu LTS 18 Cosmic Cuttlefish
 	* 18.10, cosmic-20190131, cosmic, rolling (cosmic/Dockerfile)
 - Python 2.7, Python 3.6, Ansible 2.8, Nornir 2.0
 - [Ansible 2.8 "How Many More Times"](https://github.com/ansible/ansible/blob/stable-2.8/changelogs/CHANGELOG-v2.8.rst)
  

![Docker Icon](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSWmA-f2WW29z9uI8XXgshto0EjIOUqWwrRPBnpkaeQbOpFZRuW)

[cldeluna/cosmic-moretimes image](https://hub.docker.com/r/cldeluna/cosmic-moretimes) 
  

------



Purpose built ansible image starting with Ubuntu:18.10 Cosmic Cuttlefish base and including:
- Python 2.7 (Legacy)
- Python 3.6
- ansible 2.9
- git
- yaml
- jinja2
- tree
- nano
- vim
- wget
- traceroute
- iputils-ping
- snmp
- snmp-mibs-downloader

Python Modules:
- nornir
- textfms
- netmiko
- ciscoconfparse
- argparse 
- requests
- xlrd
- openpyxl
- pandas

Repositories:
- https://github.com/cldeluna/ansible2_4_base.git
- https://github.com/cldeluna/cisco_aci.git
- https://github.com/cldeluna/cisco_ios.git


## Build

```
Claudias-iMac:cosmic-light claudia$ tree
.
├── Dockerfile
└── README.md

0 directories, 2 files
```

```
Claudias-iMac:cosmic-light claudia$ docker build -t cldeluna/cosmic-moretimes .
```

## Run

Run interactively and map a local directory /Users/claudia/Documents/docker_volume to the /ansible directory in the container.
```
Claudias-iMac:cosmic-light claudia$ docker run -v  /Users/claudia/Documents/docker_volume:/ansible -it cldeluna/cosmic-moretimes
```

## Docker Hub

```
Claudias-iMac:cosmic-light claudia$ docker tag cldeluna/cosmic-light:latest cldeluna/cosmic-heartbreak:latest
Claudias-iMac:cosmic-light claudia$ docker push cldeluna/cosmic-light
```

## Environment

![About Docker](AboutDocker.png)

![About Docker](About_iMac.png)

