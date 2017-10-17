# Service-Image-Recognition-In-DarkNet
Tor (The Onion Router) is free software and an open network that provides the anonymous communication to a server by using proxy traffic. The services that are run over the TOR Net called as a “Hidden Services” (HS). The web based services in Tor are known as Onion sites, so named because they end with “.onion”. Onion sites are hosted as Tor hidden services – a completely anonymous way to host websites. They’re part of the deep Web – an invisible part of the Web that’s not visible to search engines and normal users. It’s full of websites for users obsessed with privacy and anonymity online. The anonymity feature of Tor also provides a chance for hosting of illegal services like selling drugs, arms etc. Nowadays, many Law Enforcement Agencies are showing their interest in recognition or classification of TOR hidden services. This project can recognize a webpage as Hidden Service (mostly illegal) or no-hidden service using visual similarity.

# About Software
This software solution allows the user to recognise an input image as service image or no service image.  The solution has been developed as Representational State Transfer (REST) API based web service following the Client-Server technology. 
# Installation steps for Debian 8/ Ubuntu 14.04/16.04
This package requires Ubuntu 14.04 or Ubuntu 16.04 as the host operating system within an x86_64 architecture. The host system should have at least 512 MB of RAM available for service image recognition system.

```bash
apt-get update
apt-get install python3 python3-dev python3-pip
apt-get install python3-numpy python3-scipy python3-pil python3-decorator

dpkg -i python3-pywaveletes_0.5.2_amd64.deb
dpkg -i python3-imagehash_3.4_all.deb
```


# Compile the packages:
```bash
apt-get update
apt-get install python3 python3-dev python3-pip
apt-get install python3-numpy python3-scipy

pip3 install --upgrade pip
```

#Run the client from the terminal to list available services:
```bash
curl  -i -X GET http://localhost:1050/SIR/tasks
```

# Run the server:
```bash
python3 -m main.bin.start
```


# Launching unit tests
Go to the root folder of the repository and type:
```bash
nosetests -v
```
