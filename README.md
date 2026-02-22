# Blue-Team
<img src="https://github.com/hareekshith/blue-team-docker/blob/main/Home_CS_LAB.webp" alt="Poster"> <br>
A project created with for the people who are learning/working on the domains of blue-teams. This is like their playground, test the vulnerabilities, analyse the exploits and then fix em.

## Contents
- Kali Rolling (Acts as the attack box)
- Wazuh (Acts as the log displayer and analyser!)

## Also required by you
- Any debian based linux distro

## How to Setup?
- Clone this project <br>
```git clone https://github.com/hareekshith/blue-team-docker```
- Change your terminal directory to the folder named blue-team-docker <br>
```cd blue-team-docker```
- Make sure that docker is running <br>
```sudo dockerd (or) sudo systemctl start docker```
- Make sure that the certificates are installed for running wazuh components <br>
```sudo docker compose -f generate-indexer-certs.yml run --rm generator```
- Build and Install all the containers using docker-compose! <br>
```sudo docker compose up -d --build```
- Setup a VM with Debian based distro of your choice
- Then, configure the NAT Network for this Virtual Machine. Now you have your setup.

## How the dev wishes that you use it?
- Connect the Distro with Kali using the open ssh port in Kali
- Setup the vulnerability(s)
- View the logs in the Wazuh's Website UI (Wazuh-Dashboard/Kibana)
- Play around!

## Thanks
- <a href="https://github.com/wazuh/wazuh-docker">Wazuh's Docker Repository</a>
- Docker images of kali
- Debian 64-bit netinst ISO
